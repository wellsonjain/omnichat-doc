# 在 Shopify Plus 埋設 Omnichat Pixel

### 開始埋設之前

在開始埋設 Pixel 之前請先按照[步驟](../../features/tong-xun-qu-dao/wang-zhan-dui-hua-cha-jian/install/shopify.md)，安裝網頁對話插件於您的官網上

1. 點選左下角 Setting > 左側點選Customer events > Add custom pixel (可自行命名)
2. 放入以下代碼後點選Save 並且點選Connect

```
const script = document.createElement('script');
script.setAttribute('src', 'https://chat-plugin.easychat.co/shopifyPixel.js');
script.setAttribute('async', '');
document.head.appendChild(script);

console.log('init shopifyPixel')
window.omnichatTracker = window.omnichatTracker || [];

// page viewed
analytics.subscribe('page_viewed', (event) => {
  console.log('////////page_viewed////////')
  const documentLocation = event.context.window.location.href
  document.cookie = `__ocdl=${documentLocation}; path=/`;

  const customer = init.data.customer;
  if(customer) {
     const member = {
      memberId: customer.id,
      memberEmail: customer.email,
      memberPhone: customer.phone,
      memberName: customer.firstName,
    } 
    window.omnichatTracker.push(['init', 'config', member]);
  }

});

// product viewed
analytics.subscribe('product_viewed', (event) => {
  console.log('////////product_viewed////////')

  const product = event.data.productVariant.product;
  const price = event.data.productVariant.price;

  var item = {
    id: product.id,
    name: product.title,
    price: price.amount,
    brand: product.vendor
  }
  window.omnichatTracker.push(['event','view_product', item]);
  console.log('product_viewed event', item)

});

// added to cart
analytics.subscribe('product_added_to_cart', (event) => {
  console.log('////////product_added_to_cart////////')
  const cartLine = event.data.cartLine;

  const product = cartLine.merchandise.product;
  const price = cartLine.merchandise.price;
  const variant = cartLine.merchandise.title;
  
  const productItems = {
      id: product.id,
      name: product.title,
      quantity: cartLine.quantity,
      price: parseFloat(price.amount),
      brand: product.vendor,
      variant: variant
    };
  window.omnichatTracker.push(['event', 'add_to_cart', { items: [ productItems ]}]);
  console.log('product_added_to_cart event', productItems)

});

// checkout started
analytics.subscribe('checkout_started', (event) => {
  console.log('////////checkout_started////////')

  const checkout = event.data.checkout;

  const { lineItems } = checkout;
  const productItems = lineItems.map((item)=> {
    return {
      id: item.id,
      name: item.title,
      variant: item.variant.title,
      quantity: item.quantity,
      price: parseFloat(item.variant.price.amount)
    }
  })

  window.omnichatTracker.push(['event','checkout', {
      "items": productItems
  }]);
  console.log('checkout_started event', productItems)

});

//checkout completed
analytics.subscribe('checkout_completed', (event) => {	
  console.log('////////checkout_completed////////');

  const checkout = event.data.checkout;
  const { lineItems } = checkout;
  const items = lineItems.map(item => ({
    id: item.id,
    name: item.title,
    variant: item.variant.title,
    quantity: item.quantity,
    price: parseFloat(item.variant.price.amount)
  }));

  window.omnichatTracker.push(['event','purchase', {
      "transaction_id": checkout.order.id,
      "amount": checkout.totalPrice.amount,
      "currency": checkout.totalPrice.currencyCode,
      "items": items
  }]);

  console.log('checkout_completed event ', {
      "transaction_id": checkout.order.id,
      "amount": checkout.totalPrice.amount,
      "currency": checkout.totalPrice.currencyCode,
      "items": items
  })

});
```
