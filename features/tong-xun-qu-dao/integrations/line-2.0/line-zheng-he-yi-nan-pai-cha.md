# LINE 整合疑難排查

{% hint style="danger" %}
1. 若整合 Omnichat 之後，無法正常在 Omnichat 收到 LINE 的訊息或者無法在 Omnichat 發訊息給 LINE 帳號，請依照以下的步驟檢查是否在整合 LINE 的過程有錯誤
2. 在 LINE OA 後台回覆給客人的訊息不會進入到 Omnichat 的後台
{% endhint %}

### 1.檢查 LINE OA 後台 Messaging API 的開關狀況

進入 LINE 官方帳號後台 --> 設定 --> 回應設定，檢查 **Webhook** 是否是 **啟用**

<figure><img src="../../../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure>

### 2. 檢查 Messaging API 設定是否正確

&#x20;進入 LINE 官方帳號後台 --> 設定 --> Messaging API，檢查 Messaging API 所設定的 **Channel ID** / **Channel secret** / **Webhook** 網址是否與 Omnichat 後台的[**串接社群通訊渠道**](https://app.easychat.co/integration.html)之設定相同

![](<../../../../.gitbook/assets/line integration check 3.png>)

### 3. 進入 Line Developers 後台檢查設定是否正確

由第二點所提供的圖片上有個 LINE Developers 後台入口進入開發者後台。

進入 LINE Developers 後：

1/ 點擊右上方的頭像，並選擇你的帳號 \
2/ 選擇 Provider（服務提供者）\
3/ 選擇 Channel（官方帳號）\
4/ 進入「Basic Settings」和「Messaging API 」兩個分頁

![](<../../../../.gitbook/assets/串接 line 09.jpg>)

![LINE Developers Basic settings 設定頁面](<../../../../.gitbook/assets/螢幕快照 2019-12-31 下午12.28.56 (1).png>)

#### 檢查相關設定是否正確

&#x20;檢查 **App name** / **Channel ID** / **Channel Secret，**&#x7B49;內容是否與 Omnichat 後台的[**串接社群通訊渠道**](https://app.easychat.co/integration.html)之設定相同

![](<../../../../.gitbook/assets/line integration 2.0 -4.png>)

![](<../../../../.gitbook/assets/line integration 2.0 -5 (1).png>)

上述檢查完成後繼續檢查以下項目

1. 檢查 **Webhook URL** 是否與 Omnichat 後台的**串接社群通訊渠道**之設定相同。
2. **Use webhook 為 開啟**
3. 檢查 **Channel access token** 是否與 Omnichat 後台的**串接社群通訊渠道**之設定相同。

![](<../../../../.gitbook/assets/截圖 2024-03-13 下午5.57.53.png>)

![檢查 Channel access token 是否與 Omnichat 後台設定吻合](<../../../../.gitbook/assets/line integration 2.0 -8 (1).png>)

### 4. 進入 Line Developers 後台更新 **channel secret** 與  **access token**

如確認Line Developers 後台資訊與Omnichat 後台的**串接社群通訊渠道**之設定相同，整合串接依然失效，請至 Line developers後台重新更新 **channel secret** 與  **access token** ，複製新的**channel secret**與**access token** 到Omnichat後台『串接社群通訊渠道』，按下『更改』重新更新

![按下『Issue』取得新的Channel Secret ](<../../../../.gitbook/assets/Screen Shot 2021-09-30 at 12.29.04 PM.png>)

![按下『Reissue』取得新的Channel Secret ](<../../../../.gitbook/assets/Screen Shot 2021-09-30 at 12.29.10 PM (1).png>)







