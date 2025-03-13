---
description: 透過手機號碼比對顧客 LINE 帳號，不論是否是官方帳號好友，都可以透過 LINE 發送通知
---

# LINE 通知快捷（加購功能）

{% hint style="info" %}
若需開通該功能，請洽 Omnichat 顧問或可線上與我們聯繫。\
使用該功能前<mark style="color:red;">**請先完成 LINE 訊息 & 簡訊費用儲值**</mark>，方才能使用
{% endhint %}

## LINE 通知快捷發送流程說明

若事件發生時，在第一階段發送 LINE 通知訊息失敗時，會採以簡訊方式發送，並邀請客人加入品牌 LINE 官方帳號。

<figure><img src="../../.gitbook/assets/image (102).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
1. 目前該功能需要進行 API 串接，請依照 [API 文件](https://developers.omnichat.ai/password?redirect=/docs/send-notification-messages-to-contacts) 進行開發
2. 當品牌通知事件發生後，Omnichat 會按順序發送訊息：LINE 推送訊息、LINE 通知型訊息、簡訊
{% endhint %}

## 後台設定畫面 <a href="#membercard-setting-back" id="membercard-setting-back"></a>

### 1. 新增通知

<figure><img src="../../.gitbook/assets/截圖 2024-07-22 上午10.39.54 (1).png" alt=""><figcaption></figcaption></figure>

### 2. 基本設定 & 通知設定

<figure><img src="../../.gitbook/assets/截圖 2024-07-22 上午10.41.51.png" alt=""><figcaption></figcaption></figure>

1. 名稱：請輸入名稱（字數上限為：50 字）
2. 應用情境：請選擇應用情境

{% hint style="info" %}
1) 目前可使用的情境為：**購買完成通知、出貨通知、到貨通知、註冊完成通知、預約完成通知、預約提醒通知、帳單繳費通知、帳單預期繳費通知、維修申請通知、維修完成通知、付款完成通知、付款提醒通知、繳費完成通知、合約到期提醒、加值服務啟用通知、加值服務到期通知、開通通知等情境**（未來將持續開發）
2) 有其他通知情境的需求，歡迎向業務、客服窗口詢問
{% endhint %}

**購買完成通知**

<figure><img src="../../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>

**出貨通知**

<figure><img src="../../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure>

**到貨通知**

<figure><img src="../../.gitbook/assets/image (98).png" alt=""><figcaption></figcaption></figure>

**註冊完成通知**

<figure><img src="../../.gitbook/assets/image (99).png" alt=""><figcaption></figcaption></figure>

**預約完成通知**

<figure><img src="../../.gitbook/assets/image (436).png" alt="" width="321"><figcaption></figcaption></figure>

**預約提醒通知**

<figure><img src="../../.gitbook/assets/image (101).png" alt=""><figcaption></figcaption></figure>

**帳單繳費通知**

<figure><img src="../../.gitbook/assets/image (437).png" alt="" width="320"><figcaption></figcaption></figure>

**帳單逾期繳費通知**

<figure><img src="../../.gitbook/assets/image (438).png" alt="" width="322"><figcaption></figcaption></figure>

**維修申請通知**

<figure><img src="../../.gitbook/assets/image (439).png" alt="" width="375"><figcaption></figcaption></figure>

**維修完成通知**

<figure><img src="../../.gitbook/assets/image (440).png" alt="" width="296"><figcaption></figcaption></figure>

**付款完成通知**

<figure><img src="../../.gitbook/assets/image (427).png" alt="" width="322"><figcaption></figcaption></figure>

**付款提醒通知**

<figure><img src="../../.gitbook/assets/image (428).png" alt="" width="305"><figcaption></figcaption></figure>

**繳費完成通知**

<figure><img src="../../.gitbook/assets/image (429).png" alt="" width="328"><figcaption></figcaption></figure>

**合約到期提醒**

<figure><img src="../../.gitbook/assets/image (430).png" alt="" width="320"><figcaption></figcaption></figure>

**加值服務啟用通知**

<figure><img src="../../.gitbook/assets/image (431).png" alt="" width="329"><figcaption></figcaption></figure>

**加值服務到期通知**

<figure><img src="../../.gitbook/assets/image (432).png" alt="" width="281"><figcaption></figcaption></figure>

**開通通知**

<figure><img src="../../.gitbook/assets/image (433).png" alt="" width="284"><figcaption></figcaption></figure>

3. 通知方式

* 3-1：LINE 推送訊息
* 3-2：通知型訊息頁尾連結：請提供 URL 連結，連結須包含有關通知型訊息的說明。您可以將說明加在官網的隱私權政策中。
* 3-3：簡訊：請輸入簡訊內容，並可設定轉發簡訊的等待時間。

{% hint style="info" %}
1. 簡訊內容：簡訊內文若有使用變數，請使用雙括弧來表示，ex. \{{variable\}}，雙括弧中只能有英文、數字與底線。變數內容請在發送 API 時提供
2. 簡訊字數計算方法：上限 70 個字元（包含中文、英文、數字、空白、換行、標點符號），超過字數會分封寄送
3. 訊息若超過 70 個字元，以每 67 個字為一封簡訊
4. 使用 GSM 特殊符號 ex. (  ^ { } / \[ ] I ) 計算為兩個字元
{% endhint %}

### 3. 複製 「設定 ID 」，並依照 Open API 文件說明開發

{% hint style="info" %}
1. 目前該功能需要進行 API 串接，請依照 [API 文件](https://developers.omnichat.ai/password?redirect=/docs/send-notification-messages-to-contacts) 進行開發
2. 每一種情境都會有對應的 Setting ID，交由貴司客戶工程師前請先完成需要串接的 LINE 通知快捷情境，並將 Setting ID 提供給工程師
{% endhint %}

<figure><img src="../../.gitbook/assets/截圖 2024-07-22 上午11.02.57.png" alt=""><figcaption></figcaption></figure>

## 總覽列表頁面

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午2.08.19.png" alt=""><figcaption></figcaption></figure>

1. 總觸發數
2. 通知完成數：所有觸發中成功完成通知的數量
3. LINE 推送訊息送達數：推送訊息的送達數；LINE 推送訊息送達率：推送訊息送達數 / 推送訊息總發送數
4. LINE 通知型訊息送達數：通知型訊息的送達數；LINE 通知型訊息送達率：LINE 通知型送達數 / LINE 通知型訊息訊息總發送數
5. 簡訊送達數：簡訊的送達數；簡訊送達率：簡訊送達數 / 簡訊總發送數
6. LINE 通知型訊息加入好友數：因收到 LINE 通知型訊息而加入好友的人數
7. 簡訊加入好友數：透過簡訊的連結而加入好友的人數
8. 動作：可編輯 LINE 通知型快捷 & 複製 「 設定 ID 」

## 匯出紀錄

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午2.56.41.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午2.54.04 (1).png" alt=""><figcaption></figcaption></figure>

CSV 檔案匯出紀錄，支援的數據如下：

* 觸發 ID
* 觸發時間
* 名稱
* 應用情境
* 手機號碼
* 發送狀態（發送中 / 發送成功 / 發送失敗）
* 送達時間
* 送達方式（LINE 推送訊息 /  LINE 通知型訊息 / 簡訊）
* LINE 推送訊息發送狀態
* LINE 推送訊息送達時間
* LINE 通知型訊息發送狀態
* LINE 通知型訊息送達時間
* 簡訊發送狀態
* 簡訊送達時間
* 最後更新時間
