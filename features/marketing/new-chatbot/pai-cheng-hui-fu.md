---
description: >-
  適用平台：所有社群平台（包含 LINE)，但 WhatsApp、Facebook 和 Instagram 受24小時政策限制，網站插件（Webchat
  ）未來將開放使用
---

# 排程回覆

## 網站插件使用排程回覆卡片設定

設定一段時間內未與客戶互動後，系統將自動發送訊息給客戶。

<figure><img src="../../../.gitbook/assets/10 (1).png" alt=""><figcaption><p>排程回覆卡片設定與觸發流程</p></figcaption></figure>

1. **排程回覆卡片可設定在任一種卡片的後方。**
2. **排程發送時間（必填）：**\
   設定多久時間進行觸發，目前支援以 「 分鐘 」 計算。最小須輸入1，數字只能輸入正整數，如果輸入小數點，會直接捨棄小數點的部分。
3. **排程期間內客人互動（必選）：**
   1. 可設定當客人在觸發時間內有進行回覆時，要不要自動觸發下一個機器人模組。
   2. 互動包含：點擊機器人按鈕、傳送文字訊息、傳送圖片等等。
4. **回覆內容（必填）：**\
   選擇欲回覆給客戶的機器人模組。

{% hint style="danger" %}
**注意事項：**

1. 所有社群平台皆支援排程回覆卡片，針對網站對話（ Webchat ）未來將會開放使用
2. 在 WhatsApp、Facebook 和 Instagram 這三平台上，如客人**超過 24 小時**沒有回送訊息時， 排程回覆卡片將無法成功發送訊息（受限於 [Meta 24 小時政策](https://developers.facebook.com/docs/messenger-platform/policy/policy-overview/)），因此建議這三平台的排程發送時間不要設定超過 24 小時（1440分鐘）。
{% endhint %}
