# 遊戲模組專用—LINE LIFF ID 設定

{% hint style="info" %}
若您尚未建立過 LINE Login Channel 請您先參考[此篇教學文件說明](https://docs.omnichat.ai/features/tong-xun-qu-dao/integrations/line-2.0/she-ding-liff-id-xian-she-ding-login-channel#nothaveloginchannel)，完成建立 Login Channel 建立後再進行遊戲模組 LIFF ID 的設定
{% endhint %}

### 步驟一：

在 LINE Login channel 創建一個 LIFF 並填入資訊

1. 點選『LIFF』
2. 按下中間『Add』按鈕

![](<../../../../.gitbook/assets/截圖 2021-12-10 上午11.17.30.png>)

### **步驟二：將創建的 LIFF 填入資訊**

1. LIFF app name 填 **Omnichat 遊戲模組**
2. Size 選 **tall**
3. Endpoint URL 填：https://game.omnichat.ai/?liffId=
4. Scopes 三個選項全勾
5. Add friend option 選 On (Aggressive)
6. Scan QR 打開
7. 完成設定後請按 Add 新增 LIFF

<figure><img src="../../../../.gitbook/assets/截圖 2024-12-13 下午2.30.53.png" alt=""><figcaption></figcaption></figure>

### 步驟三：開啟 shareTargetPicker 功能

開啟時，會需要您勾選並點擊「Enable」的按鈕，即可開啟該功能

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午6.39.12.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午6.40.19.png" alt=""><figcaption></figcaption></figure>

### 步驟四：

1. 按剛剛創建的 LIFF ，進入設定頁面中的 Endpoint URL，按下「Edit」
2. 將 Endpoint URL 內「=」後加上 LIFF ID（可直接複製）
3. 點擊按鈕「Update」

Ex: [https://game.omnichat.ai/?liffId=1655713626-ljKQMJy2](https://game.omnichat.ai/?liffId=1655713626-ljKQMJy2)

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午6.45.37.png" alt=""><figcaption></figcaption></figure>

### 步驟五：請協助檢查在 LINE Login 是否有連結到您的官方帳號

{% hint style="warning" %}
請注意，如果您在該步驟沒有看到您的官方帳號資料，表示您的 LINE Login Channel 跟 LINE Messaing API Channel 沒有在相同的 Provider 之下，請到同一個 Provider 下建立 LINE Login Channel。\
\
又或者是，您目前是沒有正確的 Provider 權限，這部分需要請有權限的同仁協助完成相關建置。
{% endhint %}

請確認在 LINE Login 的 Basic Setting 頁面，拉到最下面有一個項目 「Add friend option」 ，確認 `Linked LINE Official Account` 這個欄位是有連結到貴司的 LINE 官方帳號，若沒有請點擊後完成 update !

<figure><img src="../../../../.gitbook/assets/截圖 2024-05-21 下午2.56.08.png" alt=""><figcaption><p>點擊下拉式選單，找到您的官方帳號資訊，並點擊 update</p></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/截圖 2024-05-21 下午2.56.01.png" alt=""><figcaption><p>完成 update 的樣子</p></figcaption></figure>

### 步驟六：最後一步！

到通訊渠道 -> 串接社群通訊渠道 -> 點開三個點的地方，按下「編輯」

<figure><img src="../../../../.gitbook/assets/截圖 2022-09-01 下午7.47.34.png" alt=""><figcaption></figcaption></figure>

將 LIFF ID 貼上，點擊「儲存」就大功告成！

<figure><img src="../../../../.gitbook/assets/截圖 2022-09-01 下午7.48.03.png" alt=""><figcaption></figcaption></figure>
