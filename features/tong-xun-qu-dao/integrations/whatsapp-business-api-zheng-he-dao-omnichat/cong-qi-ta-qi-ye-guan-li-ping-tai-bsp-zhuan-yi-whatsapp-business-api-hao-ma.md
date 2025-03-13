# 從其他企業管理平台(BSP)轉移 WhatsApp Business API 號碼



當您 WhatsApp Business API (WABA) 是由其他廠商（BSP）來協助申請時，您想將已使用在另一個 BSP 註冊的相同電話號碼也想在 Omnichat 中設置 WABA，您可以按照下列教學將電話號碼轉移到 Omnichat

在開始轉移之前，請注意：

* **在轉移號碼至我們的伺服器時，將會無法進行使用一段時間**&#x20;
* **官方企業帳戶(綠勾)將與電話號碼一起轉移，以及範本訊息（使用中 - 高品質）會一起轉移**
* **原有對話不會被轉移到 Omnichat**

## 轉移條件

<table data-header-hidden><thead><tr><th width="279.53787367947854">資料</th><th>轉移條件</th></tr></thead><tbody><tr><td>電話號碼</td><td><strong>1.</strong> 您的號碼需為 WhatsApp Business API 帳號且完成註冊<br><strong>2.</strong> 需請先前廠商進行禁用該號碼的雙重身份驗證（禁用6位數密碼）,且需要刪除該號碼</td></tr><tr><td>從其他廠商申請的 WABA</td><td><strong>1.</strong> 需完成 Facebook 商家驗證<br><strong>2.</strong> WABA 的審核狀態必須是Approved.</td></tr><tr><td>Omnichat 後台的 WABA</td><td><strong>1.</strong> 需完成 Facebook 商家驗證<br><strong>2.</strong> WABA 的審核狀態必須是Approved.</td></tr></tbody></table>

{% hint style="danger" %}
### **關於禁用雙重驗證，請將現有的** BSP 按照此連結操作 [**https://developers.facebook.com/docs/whatsapp/api/settings/two-factor#disable**](https://developers.facebook.com/docs/whatsapp/api/settings/two-factor#disable)&#x20;
{% endhint %}

<figure><img src="../../../../.gitbook/assets/截圖 2022-11-30 下午5.27.13.png" alt=""><figcaption></figcaption></figure>

## 創建一個新的 WABA

為了順利完成轉移，你需要先創建一個新的 WABA 帳戶，將 Omnichat 設為目的地來轉移WABA帳戶的電話號碼。如果滿足所有條件，請按照以下步驟進行轉移。

### **1. 登入** Omnichat 平台並創建 WABA  : [`https://app.omnichat.ai/integration.html`](https://app.omnichat.ai/integration.html)

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-08 下午4.50.51.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-05 下午5.58.55.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-05 下午5.53.32.png" alt=""><figcaption></figcaption></figure>

### 2-1. 創建一個新的 Meta Business 帳戶（Facebook Business Manager）和 WABA 帳戶

(1) 法定企業名稱：提交的公司名稱應與在商業登記 (BR) 文件中註冊的合法公司名稱一致 。\
(2) 營業電話：可以是手機也可以是固定電話，這個號碼不適合 WABA 應用程序。 \
(3) 企業網站：提交的公司網域應該與提交的公司名稱一致 。\
(4) 您的企業電子郵件地址：提交的公司郵件網域應與提交的公司網域一致。 \
(5) 國家和時區：選擇您的公司註冊所在的國家和時區。

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-05 下午5.49.23.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-05 下午5.50.15.png" alt=""><figcaption></figcaption></figure>

### 2-2. 選擇現有的 Meta Business 帳戶並創建新的 WABA 帳戶

(1)選擇您現有的 WhatsApp Business API 帳號並收取驗證碼即可。\
(2)此帳戶顯示名稱將顯示在 Facebook Business Manager平台上，並不是 WABA 顯示名稱唷。

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-08 下午5.26.40.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-08 下午5.30.20.png" alt=""><figcaption></figcaption></figure>

### 3. 創建您的 WhatsApp Business 資料並驗證您的 WABA 號碼

{% hint style="warning" %}
(1) WhatsApp Business API 顯示名稱應與您的商業名稱相同\
(2) 請注意 Meta 對 WhatsApp Business 顯示名稱的審核，最多可能需要等待 3 個工作日\
(3) 客人將看得到您 WhatsApp 上的商家簡介資料\
(4) 無法註冊到現有的 WhatsApp 個人 / WhatsApp Business 帳號
{% endhint %}

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-05 下午6.24.42.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-05 下午6.25.29.png" alt=""><figcaption></figcaption></figure>

### 4. 回到 Omnichat 使用者後台並刷新頁面後，恭喜您！ 您的號碼已完成接通囉。&#x20;

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-05 下午5.25.12.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/截圖 2022-12-05 下午5.25.32.png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
1. **成功綁定了 WABA 後， 要在 30 天內完成 Meta 商業驗證（位置在 Meta 的安全中心內）**
2. **在 WhatsApp 官方驗證前，每 24 小時限制只能發送 50 條 business-initiated 訊息**\
   **轉移完成後，在前廠商所建立的範本訊息無法移轉至 Omnichat，會需要重新遞交之前的申請。**
{% endhint %}

