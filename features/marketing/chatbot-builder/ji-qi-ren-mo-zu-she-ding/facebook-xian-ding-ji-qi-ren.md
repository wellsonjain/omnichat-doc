---
description: 依照各社群渠道會有不同的限定卡片可使用，當選擇發佈平台是在限定單一平台時（如 LINE 或是 Facebook 等），即有限定卡片可以使用
---

# Facebook 限定機器人

## Facebook 定期通知卡片

若需使用定期通知卡片，請先重新新增一隻機器人，並選擇「**只限 Facebook/Instagram** 」！

FB 行銷推播內容只限客人過去跟品牌 24 小時內有互動才能成功送出，如過去 24 小時沒有互動過，客人無法從 Facebook 收到品牌的推播訊息

為了解決 Facebook 推播限制，讓客人能訂閱自己想收到的訊息。Facebook 為品牌們提供 Recurring notifications (定期通知訊息)

更多詳細說明可以參考 Facebook 官方文件：[https://developers.facebook.com/docs/messenger-platform/send-messages/recurring-notifications/](https://developers.facebook.com/docs/messenger-platform/send-messages/recurring-notifications/)

### 卡片設定

<figure><img src="../../../../.gitbook/assets/截圖 2023-05-09 下午2.20.56.png" alt=""><figcaption></figcaption></figure>

1. 設定 FB 訂閱定期通知卡片
2. 上傳圖片：圖片手機版：1.94 : 1；網頁版：1.66 : 1
3. 設定主題
4. 「接收訊息」按鈕無法修改按鈕文字。（因 Facebook 限制）
5. 對話模組：設計對話模組可以導到其他模組
6. 標籤：消費者點擊後，為他們加上標籤

### Facebook 訂閱定期通知使用注意事項

推播的發送頻率為「每日一次（每 24 小時）」，若選擇訂閱，將會持續訂閱，直到客人主動取消為止。

### **活用 Facebook 定期通知**訊息

如何讓消費者可以看到機器人卡片並按下訂閱，您可以善用 Omnichat 後台相關功能來進行

#### ㄧ、[**FB Messenger 歡迎模組**](../../../tong-xun-qu-dao/automated-messages/welcome-message.md)**觸發定期通知訊息**

設定完機器人後，進到社群渠道設定—歡迎訊息選擇該機器人模組。消費者按下『開始使用』後可以透過歡迎模組，來訂閱定期通知訊息，讓客人能訂閱自己想收到的訊息

![](<../../../../.gitbook/assets/截圖 2022-06-20 下午4.15.27.png>)

#### **二**、[**Facebook 主選單（常設功能表）**](../../../tong-xun-qu-dao/automated-messages/chang-she-gong-neng-biao.md)**觸發定期通知型訊息**

![](<../../../../.gitbook/assets/截圖 2022-06-20 下午3.17.31.png>)

![](<../../../../.gitbook/assets/截圖 2022-06-20 下午4.54.54.png>)

#### 三、**Facebook 貼文 的 CTA 觸發訂閱通知訊息**

先設定關鍵字如：「我要訂閱」、「訂閱」，然後藉由 [關鍵字自動回覆](../../keyword-autoreply.md) 設定來讓客人輸入關鍵字後訂閱定期通知訊息

![](<../../../../.gitbook/assets/截圖 2022-03-30 下午6.44.50.png>)

#### 四、**Facebook 貼文留言功能觸發定期通知訊息**

您可以在 Facebook 粉專上發佈一篇引導定期通知訊息的貼文，並給予有完成訂閱的客人回饋

* 設定完定期通知訓息機器人卡片後，多設定一個機器人模組來導向 FB 定期訊息機器人
* 將該貼文私訊回覆，設定為剛剛設定的機器人模組。

![](<../../../../.gitbook/assets/截圖 2022-03-30 下午6.52.55.png>)

您也可以設計導向的對話模組內含有誘因（如優惠券代碼、贈品等），提高消費者訂閱意願

![](<../../../../.gitbook/assets/截圖 2022-03-30 下午6.55.40.png>)

#### 五、**在**[**遊戲模組**](../../../you-xi-mo-zu-jia-gou-gong-neng/)**中設定觸發定期通知訊息**

當客人遊玩遊戲模組時，可以設計其中一個獎項是觸發定期通知**FB recurring notifications**訊息，讓中獎的客人進一步訂閱

<figure><img src="../../../../.gitbook/assets/教學文章_FB 定期訂閱通知.jpg" alt=""><figcaption></figcaption></figure>

![](<../../../../.gitbook/assets/截圖 2022-03-30 下午7.01.53.png>)



## Facebook 連結觸發（m.me 連結） <a href="#lian-jie-chu-fa-mme-lian-jie" id="lian-jie-chu-fa-mme-lian-jie"></a>

連結觸發讓消費者可以同時完成「打開粉專 Messenger」與「觸發特定對話模組」。讓客人可從外部連結直接導向 Facebook Messenger 的對話模組，也可以適用於線下活動哦！

{% hint style="info" %}
關於 Mata 官方說明 m.me 連結設定方式，請參考此份文件：[https://developers.facebook.com/docs/messenger-platform/discovery/m-me-links/?locale=zh\_HK](https://developers.facebook.com/docs/messenger-platform/discovery/m-me-links/?locale=zh_HK)
{% endhint %}

### 步驟一：設定您專屬的 m.me 連結 <a href="#fbmme" id="fbmme"></a>

依據 FB 官方的說明文件表示，m.me 的專屬連結，可以使用 `http://m.me/PAGE-NAME` 此段連結進行設定，其中 <mark style="color:blue;">**「PAGE-NAME」**</mark>為您的 Facebook 粉絲專頁網址後的代碼 。

以下圖為例，該粉絲專頁的 PAGE-NAME 就是：**「onlyoneyou」**：

![在 FB 粉絲專頁的網址列](<../../../../.gitbook/assets/截圖 2023-03-28 下午2.12.27.png>)

或者您也可以到粉絲專頁的設定位置：[https://www.facebook.com/settings/?tab=pages](https://www.facebook.com/settings/?tab=pages)，找到 「粉絲專頁設定」、點入「姓名」欄位，即可看到粉絲專頁的用戶名稱為onlyoneyou， m.me 連結則為：<mark style="background-color:orange;">**http://m.me/onlyoneyou.**</mark>

<figure><img src="../../../../.gitbook/assets/m.me連結.png" alt=""><figcaption><p>在粉絲專頁設定查詢自己的用戶名稱</p></figcaption></figure>

### 步驟二：複製需要導向的機器人模組 ID

進到您想觸發的機器人模組內，複製『block-id』後面的那一串編碼

![](<../../../../.gitbook/assets/截圖 2023-03-28 下午2.56.19.png>)

### 步驟三：將 m.me 連結與機器人的 block-id 組合起來。

公式：「m.me 連結」＋「?ref=」+「block-id=後面的數字編碼」

<mark style="color:red;">EX：http://m.me/onlyoneyou?ref=efef7579-e71f-4a10-bb30-73bf56672306</mark>

{% hint style="info" %}
請注意網址連結請勿使用粗體字體，會影響到連結的跳轉。
{% endhint %}

### 步驟四：可以將組成好的連結放在 E-mail、EDM、外部網站或是線下活動進行等來做使用

<figure><img src="../../../../.gitbook/assets/截圖 2023-03-28 下午2.58.24.png" alt=""><figcaption></figcaption></figure>

## 注意事項

{% hint style="info" %}
Faceboook 官方於 2022 年推出該功能，關於使用上的相關政策，可參考以下說明網頁：[https://developers.facebook.com/docs/messenger-platform/send-messages/recurring-notifications/](https://developers.facebook.com/docs/messenger-platform/send-messages/recurring-notifications/)
{% endhint %}

#### 1. Facebook 官方有機會會提前發出「Continue messages」提供給消費者

#### 2. 消費者可以隨時到 Messenger App 內管理訂閱通知，包含「取消」和「恢復」。

![消費者訂閱之後又停止接收訊息](<../../../../.gitbook/assets/截圖 2022-06-24 下午4.56.57.png>)

### &#x20;對已經點擊 Facebook 定期通知客人推播時

#### 1. 請留意，雖然可透過定期通訊息聯繫消費者，但仍有一定的機會/其他因素，導致推播訊息時產生失敗的情形。舉例來說：若 Facebook 粉絲專頁的互動率（不重複每日活躍用戶）過低時，FB官方針對該情況有相關限制，導致無法成功推播訊息。

<figure><img src="../../../../.gitbook/assets/截圖 2022-09-30 下午3.48.52.png" alt=""><figcaption></figcaption></figure>

#### 2. **Facebook 官方文件中有提出限制，針對同一位消費者，在 7 天內最多可發送 10 次訂閱定期通知卡片的提醒，在 1 天內最多可發送 5 次訂閱定期通知卡片的提醒，若您 Facebook 粉絲專頁互動率過低，有機會減少上述所提及的可發送次數**

#### 3. 推播時，您會需要再勾選以下兩個條件為「是」，並且為「訂閱中」來進行篩選才是這個時間可以使用定期通知來推播的人數唷

<figure><img src="../../../../.gitbook/assets/截圖 2022-11-08 下午3.25.37.png" alt=""><figcaption></figcaption></figure>

#### 4.  如您是要對已經訂閱 Facebook 定期通知的客人使用機器人模組來推播，請留意機器人模組內僅能含有一張機器人卡

如您機器人模組內有第二張以上（包含第二張）機器人卡片，文字或是圖片，則會改為一般標準訊息來發送，就會受到 [Facebook 24 政策限制](https://developers.facebook.com/docs/messenger-platform/policy/policy-overview/)

