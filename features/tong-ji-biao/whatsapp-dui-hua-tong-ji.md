---
description: 此功能限有購買 WhatsApp Business API 方案用戶使用
---

# WhatsApp 對話統計

WhatsApp 的對話統計頁面會顯示免費與付費的對話數量，並以圖表呈現付費對話總數費用。而在此統計表當中的數值為<mark style="color:red;">**近似值**</mark>，實際收費請以每月所收到的 WhatsApp 對話費用明細為準。

以下針對該頁面當中會呈現的數據逐一進行說明

### 日期區間 <a href="#day" id="day"></a>

<figure><img src="../../.gitbook/assets/截圖 2023-03-13 下午5.30.10.png" alt=""><figcaption></figcaption></figure>

* 一開始進到該頁面的預設日期，是從當天開始計算到過去的 14 天（兩週）
* 可點選日期，去篩選特定日期區間的數據
* 搜尋新日期區間後，整個頁面的數據會同時一起更新
* 當日數據更新頻率為：每小時/次
* 「所有地區」可篩選特定地區的聊天統計對話量，分為：全部地區、亞洲地區、非亞洲地區
* 最左側呈現有串接到 Omnichat 的 WhatsApp Business API （以下簡稱為 WABA）的電話號碼，若有串接多支電話號碼可從下拉式選單中篩選需要查看的 WABA 帳號

### 左側對話量統計說明 <a href="#leftconversationwaba" id="leftconversationwaba"></a>

<div align="left"><figure><img src="../../.gitbook/assets/截圖 2023-06-08 上午10.08.42.png" alt="" width="228"><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/截圖 2023-06-08 上午10.11.28 (1).png" alt="" width="228"><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/截圖 2023-06-08 上午10.13.42.png" alt="" width="229"><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/截圖 2023-06-08 上午10.14.35.png" alt="" width="229"><figcaption></figcaption></figure></div>

_可點擊上方圖片放大檢視_

2023/06/01起，WhatsApp Business API的對話收費方式中&#x7684;**「商家發起」**，將細分&#x70BA;**「公用對話」**、**「驗證對話」**、**「行銷對話」等3種對話，「用戶發起」**&#x5C07;會屬&#x65BC;**「服務對話」**&#x4E0D;同類別的對話會有不同對話費率，因此在對話統計表當中將會呈現是由哪一種對話的相關資料

關於收費的方式，2024/11/01 WhatsApp 官方有針對新的計費方式公布相關做法，可先參考[此篇文件的說明](https://blog.omnichat.ai/hk/whatsapp-business-api-new-pricing-update-2024-zh/)

* 所有對話 = **「公用對話」**、**「驗證對話」**、**「行銷對話」**、**「服務對話」**&#x7684;總訊息數
* 免費期間/免費服務對話 = 自 2024 年 11 月 1 日起，由用戶開啟的服務對話皆為免費，不限於1,000則訊息。只要是顧客先發起對話，Meta 在 24 小時內將不會向同一對話的工具範本訊息收費，企業可以無限次免費發送重要通知，如訂單確認、預約提醒或通知等，增進與顧客的緊密度。
* 免費進入點 (Free Entry Point Conversations) = 當**客人端**透過，廣告當中置入 WhatsApp 行動呼籲按鈕（Call to Action) 或是在 Facebook 粉絲專頁當中放上 WhatsApp 的行動呼籲按鈕**來與商家端進行訊息互動**，該訊息即屬於免費入口點對話，該筆對話將不會產生訊息費用。\
  <mark style="color:blue;">**＊注意事項：免費進入點對話會持續72小時，且只能由用戶主動開啟。過了72小時後，用戶再持續跟商家對話需要收費**</mark>
* 付費對話 = 包&#x542B;**「公用對話」**、**「驗證對話」**、**「行銷對話」**、**「服務對話」**&#x9019;四種需收費訊息對話的統計數
* 費用 = 此處將以團隊所在地區顯示訊息費用，計算包&#x542B;**「公用對話」**、**「驗證對話」**、**「行銷對話」**、**「服務對話」**&#x9019;四種需收費訊息對話的金額總計

### 右側對話圖表統計說明 <a href="#rightconversationwaba" id="rightconversationwaba"></a>

下列圖表均可以透&#x904E;**「下載 CSV」**&#x6A94;案的功能匯出相關日期區間報表，可參考下圖範例

<figure><img src="../../.gitbook/assets/截圖 2023-06-08 上午10.37.45.png" alt=""><figcaption></figcaption></figure>

檔案中欄位包含：日期、WABA 帳號號碼、所在地區、國碼、發起對話方、訊息類型（免費/付費）、訊息數量、費用等欄位可進行查看

<figure><img src="../../.gitbook/assets/截圖 2023-06-08 上午10.44.26.png" alt=""><figcaption></figcaption></figure>

* （商家發起）公用對話（藍色線）：
* （商家發起）驗證對話（紫色線）：
* （商家發起）行銷對話（綠色線）：
* （用戶發起）服務對話（橘色線）：

<figure><img src="../../.gitbook/assets/截圖 2023-06-08 上午10.48.09.png" alt=""><figcaption></figcaption></figure>

* 免費期間對話：為 WhatsApp Business API 每個月免費訊息數量使用狀況總計（綠色線）
* 免費進入點：為用戶端透過廣告上的行動呼籲按鈕（ Call to Action）或 Facebook 粉絲專頁中的 WhatsApp 行動呼籲按鈕傳送的訊息數量總計（紫色線）

<figure><img src="../../.gitbook/assets/截圖 2025-01-09 下午1.19.36.png" alt=""><figcaption></figcaption></figure>

* 付費對話：包含&#x7531;**「公用對話」**、**「驗證對話」**、**「行銷對話」**、**「服務對話」**&#x7684;<mark style="color:blue;">**訊息數量總計**</mark>
* 費用：以商家端所在地區呈現幣值，包含由**公用對話」**、**「驗證對話」**、**「行銷對話」**、**「服務對話」**&#x7684;<mark style="color:blue;">**總訊息費用**</mark>
