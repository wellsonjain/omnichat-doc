# 網站用戶行為追蹤

{% hint style="danger" %}
**注意，此文件只適用於工程師，如閣下並非工程師，請把這文件交給工程師以安裝到網站。**
{% endhint %}

{% hint style="info" %}
追蹤代碼埋放完成後可至 [Pixel 紀錄](https://console.omnichat.ai/pixel-record) 頁面查看 Omnichat 是否正確收到事件
{% endhint %}

如您是使用 Shopify 網站，請點擊以下連結來進行操作：

{% content-ref url="zai-shopify-plus-mai-she-omnichat-pixel.md" %}
[zai-shopify-plus-mai-she-omnichat-pixel.md](zai-shopify-plus-mai-she-omnichat-pixel.md)
{% endcontent-ref %}

## 使用入門

**使用前，請先根據 「**[**安裝對話插件**](https://docs.omnichat.ai/features/tong-xun-qu-dao/wang-zhan-dui-hua-cha-jian/install)**」，把 Omnichat 的 Javascript 插件安裝到你的官網。**

## 網站基本會員資料

| 參數               | 類型     | 必須提供 |
| ---------------- | ------ | ---- |
| memberId         | string | 否    |
| memberEmail      | string | 否    |
| memberPhone      | string | 否    |
| memberName       | string | 否    |
| memberProfilePic | string | 否    |

安裝插件後，可以透過以下方法啓動網站行為追蹤。

&#x20;將以下 Javascript 代碼方置到網站所有頁面 **\</body>** 之前:

```javascript
<script type="text/javascript">
    // OMNICHAT TRACKER V1.0
    window.omnichatTracker = window.omnichatTracker || [];
    window.omnichatTracker.push(['init', 'config', {
        "memberId": "<LOGGED-IN-MEMBER-ID>",
        "memberEmail": "<LOGGED-IN-MEMBER-EMAIL>",
        "memberPhone": "<LOGGED-IN-MEMBER-PHONE-NUMBER>",
        "memberName": "<LOGGED-IN-MEMBER-NAME>",
        "memberProfilePic": "<LOGGED-IN-MEMBER-PROFILE-PICTURE-URL>"
    }]);
</script>
```

啓動網站行為追蹤時，你可以選擇提交會員姓名、會員編號、電郵或電話，資料會在後台顯示，有利於查找對應的會員。

* 取代 **\<LOGGED-IN-MEMBER-ID>** 為網站上已登入會員的編號。如果是訪客或沒有相關資料，可以漏空。
* 取代 **\<LOGGED-IN-MEMBER-EMAIL>** 為網站上已登入會員的電郵。如果是訪客或沒有相關資料，可以漏空。
* 取代 **\<LOGGED-IN-MEMBER-PHONE-NUMBER>** 為網站上已登入會員的電話號碼(**必需加上國碼，例如：852、886，否則有機會無法綁定會員資料**)。如果是訪客或沒有相關資料，可以漏空。
* 取代 **\<LOGGED-IN-MEMBER-NAME>** 為網站上已登入會員的姓名。如果是訪客或沒有相關資料，可以漏空。
* 取代 **\<LOGGED-IN-MEMBER-PROFILE-PICTURE>** 為網站上已登入會員的大頭貼網址。如果是訪客或沒有相關資料，可以漏空。

## 電子商務追蹤

### 介紹

透過我們的 Javascript 插件，你可以追蹤到你的訪客及會員的電子商務行為，並可以在 OmniChat 的後台查閱報表及針對用戶行為設定行銷訊息。

{% hint style="warning" %}
提醒您，埋放商品數據中 pixel 資料裏面的商品 id，必須與產品目錄裡的商品 id 一致
{% endhint %}

### 商品數據

在傳送與商品相關的事件(加入購物車、結帳等)時，可以傳送以下的參數:

| 參數       | 類型      | 必須提供 | 說明          |
| -------- | ------- | ---- | ----------- |
| id       | string  | 是    | 商品的唯一編號/SKU |
| name     | string  | 是    | 商品名稱        |
| brand    | string  | 否    | 商品的品牌       |
| category | string  | 否    | 商品類別        |
| variant  | string  | 否    | 商品款式        |
| quantity | integer | 否    | 商品數量        |
| price    | number  | 否    | 商品單價        |

### 訂單數據

在傳送與訂單相關的事件(購買完成)時，可以傳送以下的參數:

| 參數              | 類型     | 必須提供 | 說明       |
| --------------- | ------ | ---- | -------- |
| transaction\_id | string | 是    | 訂單編號     |
| amount          | number | 是    | 訂單總額     |
| currency        | string | 否    | 訂單結帳貨幣單位 |

### 追蹤查看商品頁

要追蹤查看商品頁的次數，請發送以下 `view_product` 的事件:

```javascript
window.omnichatTracker.push(['event','view_product', {
    "id": "P12345",
    "name": "Android Warhol T-Shirt",
    "brand": "Google",
    "category": "Apparel/T-Shirts",
    "variant": "Black",
    "price": '2.0'
}]);
```

* 應用例子：進入商品資料頁時運行以上 Javascript (放在 \</body> 前)

### 追蹤加入購物車

要追蹤加入購物車的行為，請發送以下 `add_to_cart` 的事件:

```javascript
window.omnichatTracker.push(['event','add_to_cart', {
    "items": [
        {
            "id": "P12345",
            "name": "A Black T-Shirt",
            "brand": "Brand B",
            "category": "Apparel/T-Shirts",
            "variant": "Black",
            "quantity": 2,
            "price": '2.0'
        }
    ]
}]);
```

* 應用例子：客人在網站上點擊「加入購物車」按鈕 (可參考以下 Javascript 範例)

```javascript
// 需要替換 "add-to-cart-button" 為網站上「加入購物車」按鈕的 ID
document.getElementById("add-to-cart-button").addEventListener('click', function(e) {
    window.omnichatTracker.push(['event','add_to_cart', {
        "items": [
            {
                "id": "P12345",
                "name": "A Black T-Shirt",
                "brand": "Brand B",
                "category": "Apparel/T-Shirts",
                "variant": "Black",
                "quantity": 2,
                "price": '2.0'
            }
        ]
    }]);
});
```

### 追蹤從購物車移除商品

要追蹤從購物車移除商品的行為，請發送以下 `remove_from_cart` 的事件:

```javascript
window.omnichatTracker.push(['event','remove_from_cart', {
    "items": [
        {
            "id": "P12345",
            "name": "A Black T-Shirt",
            "brand": "Brand B",
            "category": "Apparel/T-Shirts",
            "variant": "Black",
            "quantity": 1,
            "price": '2.0'
        }
    ]
}]);
```

* 應用例子：客人在網站上點擊「移除商品」按鈕 (可參考以下 javascript 範例)

```javascript
// 需要替換 "remove-product" 為網站上「移除商品」按鈕的 ID
document.getElementById("remove-product").addEventListener('click', function(e) {
    window.omnichatTracker.push(['event','add_to_cart', {
        "items": [
            {
                "id": "P12345",
                "name": "A Black T-Shirt",
                "brand": "Brand B",
                "category": "Apparel/T-Shirts",
                "variant": "Black",
                "quantity": 2,
                "price": '2.0'
            }
        ]
    }]);
});
```

### 追蹤結帳情況

要追蹤結帳情況的行為，請發送以下 `checkout` 的事件:

```javascript
window.omnichatTracker.push(['event','checkout', {
    "items": [
        {
            "id": "P12345",
            "name": "A Black T-Shirt",
            "brand": "Brand B",
            "category": "Apparel/T-Shirts",
            "variant": "Black",
            "quantity": 1,
            "price": '2.0'
        },
        {
            "id": "P67890",
            "name": "A Red T-Shirts",
            "brand": "Brand A",
            "category": "Apparel/T-Shirts",
            "variant": "Red",
            "quantity": 2,
            "price": '3.0'
        }
    ]
}]);
```

* 應用例子：進入結帳頁時運行以上 Javascript (放在 \</body> 前)

### 追蹤購買完成

要追蹤購買完成的行為，請發送以下 `purchase` 的事件:

```javascript
window.omnichatTracker.push(['event','purchase', {
    "transaction_id": "ORDER123456",
    "amount": "7.0",
    "currency": "TWD",
    "items": [
        {
            "id": "P12345",
            "name": "A Black T-Shirt",
            "brand": "Brand B",
            "category": "Apparel/T-Shirts",
            "variant": "Black",
            "quantity": 1,
            "price": '2.0'
        },
        {
            "id": "P67890",
            "name": "A Red T-Shirts",
            "brand": "Brand A",
            "category": "Apparel/T-Shirts",
            "variant": "Red",
            "quantity": 2,
            "price": '3.0'
        }
    ]
}]);
```

* 應用例子：客人完成結帳時，載入完成結帳頁面時運行以上 Javascript (放在 \</body> 前)
