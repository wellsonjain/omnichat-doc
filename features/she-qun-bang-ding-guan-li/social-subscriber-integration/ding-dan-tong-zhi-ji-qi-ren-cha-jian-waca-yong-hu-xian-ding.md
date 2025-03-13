---
description: >-
  當您是使用 WACA
  開店平台商時，您可以使用訂單通知機器人插件。當客人完成訂單進到訂單完成畫面，透過點擊機器人按鈕，訂單狀態產生變更時，系統自動透過平台傳到消費者的社群中（Facebook、LINE）
---

# 訂單通知機器人插件（WACA 用戶限定）

### Omnichat 後台設定

#### 1.  **進入社群身份綁定頁面**

**2. 選擇「WACA訂單通知機器人」**

**3. 啟用訂單通知機器人按鈕**

**4. 選擇接收訊息的平台（Facebook / LINE）及相對應官方帳號**

{% hint style="info" %}
1. 選擇 Facebook 平台發送訂單通知訊息仍會受到 Facebook 24 小時政策影響
2. 選擇 LINE 官方帳號發送訂單通知訊息則為「Push API」訊息類型，需要收推播訊息費用
{% endhint %}

<figure><img src="../../../.gitbook/assets/截圖 2022-09-08 下午1.46.53.png" alt=""><figcaption></figcaption></figure>

#### 5.  您可以編輯標題和描述來提醒客人並點擊按鈕

#### 6.設定完成點擊訂單通知機器人流程後會收到的成功訊息

<figure><img src="../../../.gitbook/assets/截圖 2022-09-08 下午1.50.25.png" alt=""><figcaption></figcaption></figure>

### 消費者端訂單機器人按鈕流程

當消費者完成訂單時，會在右下角出現該按鈕，當客人點擊後，會出現六位數驗證碼。\
點擊按鈕連動到 LINE 官方帳號，送出六位數驗證碼，收到成功訊息。\
\{{orderId\}} 會隨著每次訂單編號不同而有所變動。

![](<../../../.gitbook/assets/截圖 2022-08-10 上午11.18.38.png>)

{% hint style="warning" %}
1. 每次訂單完成都會需要消費者點擊連結，方能對這筆訂單狀態變更發送通知
2. 點擊連結訂單通知機器人流程完成後也等於完成社群身份綁定
{% endhint %}

#### WACA 後台可對九種訂單狀態變更情境來進行自動推播，設定場景會在 WACA 後台設定。

-> [WACA 教學文件請點我](https://www.waca.net/support/id/161#orderbotplugin)
