---
description: Shopping Behavior
---

# 購物行為 2.0

### 收益與轉換率表

<figure><img src="../../../.gitbook/assets/截圖 2025-07-03 下午5.32.38.png" alt=""><figcaption></figcaption></figure>

1. 所有來源（All Sources）：全部 UTM source / medium 的資料
2. Omnichat 來源：
   * 任何有 "Omnichat" 相關字的 UTM source / medium 的資料會聚集在這裡
   * 舉例：機器人模組、官網顧客行銷、購物車再行銷、LINE 圖文選單
   * 該數據也包含在 “所有來源" 之中
3.  Omnichat 數據佔全部的佔比

    * **`( Omnichat 來源帶來的收益 / 所有來源帶來的收益 ) * 100`**
    * ( $936,306 / $1,293,243 ) \* 100 = 72.40%

    &#x20;       \= 所有收益之中，有 72.40% 是來自於 Omnichat 相關 UTM &#x20;
4. 轉換率（Conversion Rate）
   * **`完成結帳數 / 工作階段開始數 * 100`**
   * 完成結帳數：進入到 **“階段 4 - 完成交易"** 的工作階段
   * 此表格的轉換率，對應下方轉換率漏斗的 「完成結帳的工作階段」 的轉換率數據

### 轉換率漏斗

<figure><img src="../../../.gitbook/assets/截圖 2025-07-08 下午6.32.59.png" alt=""><figcaption></figcaption></figure>

* **階段 1：工作階段開始**
* **階段 2：加入購物車的工作階段**
  * 當一個工作階段開始之後，只要有把任何東西加到購物車，就會產生 「加入購物車的工作階段」
* **階段 3：開始結帳**
  * 當在購物車頁面，進入到開始結帳程序，就會產生 「開始結帳的工作階段」
* **階段 4：完成結帳的工作階段**
  * 當確定完成交易，有訂單編號後，就會產生「完成交易的工作階段」

{% hint style="info" %}
「有結帳」跟「完成交易」差別是什麼？有時候開始結帳，但在輸入個人資料（地址、付款方式等）過程中就放棄的，就不會進行到「完成交易」
{% endhint %}

#### 1. 長條圖的數據怎麼讀？

* 以綠色的所有來源（All Sources）來看，在期間內：
  * 網站有 10,352 個工作階段
  * 那在這 10,352 裡面，有 503 個工作階段**把商品加入購物車**
  * 200 個工作階段**進入到結帳的程序**
  * 145 個工作階段**確定完成交易**
* 長條圖這裡，每一步轉換率的分母都是「所有工作階段」
* 當有 364 個工作階段一路執行到**完成交易**，那轉換率就是 **`( 364 / 1,000 ) = 36.4%`**
* 這個 36.4% 就是長條圖最右邊（也是最後一個階段）的轉換率％，同時也是右上角表格裡面顯示的轉換率％

#### 2. 轉換率

<figure><img src="../../../.gitbook/assets/截圖 2025-07-08 下午6.38.52.png" alt=""><figcaption></figcaption></figure>

* 轉換率計算公式：
  * <mark style="color:red;">**( xxx 工作階段 / 所有工作階段 ) \* 100 = xxx 的轉換率％**</mark>
* 以綠色的所有來源（All Sources）來看轉換率％
  *   ( 加入購物車 / 所有工作階段 ) \* 100 = 加入購物車的轉換率％

      **`( 503 / 10352 ) * 100 = 4.86%`**
  *   ( 開始結帳 / 所有工作階段 ) \* 100 = 開始結帳的轉換率％

      **`( 200 / 10352 ) * 100 = 1.93%`**
  *   ( 完成結帳 / 所有工作階段 ) \* 100 = 完成結帳的轉換率％

      **`( 145 / 10352 ) * 100 = 1.40%`**

#### 3. 階段轉換率

<figure><img src="../../../.gitbook/assets/截圖 2025-07-08 下午6.40.38.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
「階段轉換率」 與 「轉換率」 的差異

* 「轉換率」 的分母固定都是 **所有工作階段** 的數據
* 「階段轉換率」 的分母是 **前一個階段** 的數據
{% endhint %}

* 階段轉換率計算公式：
  * <mark style="color:red;">**( 本階段的工作階段數據 / 前一個階段的工作階段數據 ) \* 100 = 本階段的階段轉換率％**</mark>
* 以綠色的所有來源（All Sources）來看
  * ( 加入購物車的 / 所有工作階段 ) \* 100 = 加入購物車的階段轉換率％\
    &#xNAN;**`( 503 / 10352 ) * 100 = 4.86%`**
  *   ( 開始結帳的工作階段 / 有放進購物車的 ) \* 100 = 開始結帳的階段轉換率％

      **`( 200 / 503 ) * 100% = 39.76%`**
  *   ( 完成結帳的 / 有結帳的 ) \* 100 = 完成結帳的階段轉換率％

      **`( 145 / 200 ) * 100 = 72.50%`**



### Omnichat 數據佔全部的佔比

<figure><img src="../../../.gitbook/assets/截圖 2025-07-08 下午6.52.59.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/截圖 2025-07-08 下午6.47.23.png" alt=""><figcaption></figcaption></figure>

* Omnichat 數據佔全部的佔比計算公式：**(&#x20;**<mark style="color:purple;">**Omnichat**</mark>**&#x20;的數據 /&#x20;**<mark style="color:green;">**所有來源**</mark>**的數據 ) \* 100**&#x20;
  * <mark style="color:red;">工作階段開始</mark>來源佔比 =（<mark style="color:purple;">**Omnichat**</mark> <mark style="color:red;">工作階段開始</mark> / <mark style="color:green;">**所有來源**</mark> <mark style="color:red;">工作階段開始</mark>）\* 100\
    &#xNAN;**`( 416 / 10352 ) * 100 = 4.02%`**
  * <mark style="color:red;">加入購物車</mark>來源佔比 =（<mark style="color:purple;">**Omnichat**</mark> <mark style="color:red;">加入購物車</mark> / <mark style="color:green;">**所有來源**</mark> <mark style="color:red;">加入購物車</mark>）\* 100\
    &#xNAN;**`( 78 / 503 ) * 100 = 15.51%`**
  * <mark style="color:red;">開始結帳</mark>來源佔比 =（<mark style="color:purple;">**Omnichat**</mark> <mark style="color:red;">開始結帳</mark> / <mark style="color:green;">**所有來源**</mark> <mark style="color:red;">開始結帳</mark>）\* 100\
    &#xNAN;**`( 38 / 200 ) * 100 = 19.00%`**
  * <mark style="color:red;">完成結帳</mark>來源佔比 =（<mark style="color:purple;">**Omnichat**</mark> <mark style="color:red;">完成結帳</mark> / <mark style="color:green;">**所有來源**</mark> <mark style="color:red;">完成結帳</mark>）\* 100\
    &#xNAN;**`( 25 / 145 ) * 100 = 17.24%`**



