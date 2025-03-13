---
description: 串接完成後，可以將聯絡人資料異動單向/雙向同步，並且當顧客在 LINE 點擊機器人按鈕前往網站時，將 LINE UID 分享給 Insider
---

# 串接 Insider

需滿足以下方案條件，才可進行 Omnichat 與 Insider 資料同步。

Omnichat 方案要求：

* 需加購 Insider CRM 模組

Insider 方案：

* 需包含 Architect



### 開始串接與授權

在 Omnichat 選單中找到串接頁面：「通訊渠道  >  串接應用程式」，並點擊 Insider 的串接按鈕。

<figure><img src="../../../.gitbook/assets/截圖 2024-04-15 下午6.49.47.png" alt=""><figcaption></figcaption></figure>

點選串接後，會跳出說明頁面，點擊開始填入資訊進行串接

API Key：在 Insider 選擇 Unified Customer Database 來產生 API KEY

<div><figure><img src="../../../.gitbook/assets/截圖 2024-04-15 下午6.52.42.png" alt=""><figcaption></figcaption></figure> <figure><img src="../../../.gitbook/assets/截圖 2024-04-15 下午6.52.56.png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
填寫後，即可完成 Insider 的串接，達成資料的單向同步（Omnichat 同步到 Insider）。

若需要雙向同步資料，需另外設定 Contact API。或是透過 Message API 透過 Omnichat 發送訊息。
{% endhint %}
