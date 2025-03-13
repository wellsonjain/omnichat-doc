---
description: 完成與 SHOPLINE 的串接後，可以將客人的會員資料透過 「自訂屬性」 的格式儲存在 Omnichat 中使用
---

# 串接 SHOPLINE

{% hint style="info" %}
相關自訂屬性定義請洽詢 「SHOPLINE」
{% endhint %}

需滿足以下方案條件，才可進行 Omnichat 與 SHOPLINE 的串接。

Omnichat 方案要求：

* 需加購 CRM 會員模組

SHOPLINE 方案：

* 須支付 SHOPLINE Apps Store 安裝費，方可從 SHOPLINE Apps Store 串接

### 步驟一

從 SHOPLINE 後台的 擴充功能商店，找到 「Omnichat 全通路會員模組」 的頁面，並點擊 「立即安裝」

<figure><img src="../../../.gitbook/assets/截圖 2024-03-19 下午2.44.07.png" alt=""><figcaption></figcaption></figure>

### 步驟二

同意條款並安裝與授權

<figure><img src="../../../.gitbook/assets/截圖 2024-03-19 下午3.40.23.png" alt="" width="432"><figcaption></figcaption></figure>

### 步驟三

點擊 「打開擴充功能」 進行串接，點擊後會轉換到 Omnichat 登入頁面，請您登入已經完成購買 CRM 模組的帳號後台，並使用管理員帳號進行串接

<figure><img src="../../../.gitbook/assets/截圖 2024-03-19 下午3.41.20.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/截圖 2024-03-19 下午5.27.03.png" alt="" width="295"><figcaption></figcaption></figure>

### 步驟四

選擇要同步會員資料的 LINE 官方帳號

{% hint style="info" %}
在此設定的 LINE 綁定渠道的「LINE 官方帳號」須與 SHOPLINE 後台 LINE 註冊及登入的「LINE 官方帳號」相同，才可成功在 Omnichat 綁定會員及 LINE 渠道身份
{% endhint %}

<figure><img src="../../../.gitbook/assets/截圖 2024-03-19 下午6.40.10.png" alt=""><figcaption></figcaption></figure>

### 步驟五

完成 LINE 官方帳號設定後，會彈出 「已成功編輯資料」 的提醒，便可以進行首次 「同步資訊」，同步後會將目前有使用 LINE 快速登入以及有手機號碼的會員資料同步到對應客人的 LINE 事件上。（資料會同步到Omnichat的**LINE社群聯絡人**上）

串接設定完成後，即可前往自訂屬性查看同步的會員資料，\
後續再視您是否有購買會員卡模組，可繼續前往設定手機綁定、會員卡。

<figure><img src="../../../.gitbook/assets/截圖 2024-03-19 下午6.11.31.jpeg" alt=""><figcaption></figcaption></figure>

### 注意事項

若您在串接過程中遇到問題，請根據顯示的提示內容進行排查，以下提供相關提示的介紹

1. 顯示提示：尚未購買 CRM 模組
   * 欲串接團隊尚未購買 CRM 模組，則無法成功串接，需與客服聯繫獲得進一步協助
   * 若選擇錯誤團隊則請重新登入選擇其他團隊串接
2.  顯示提示：此帳號無串接權限

    若登入的帳號非主管或管理員，則無法進行串接功能，請重新登入有權限的帳號以利串接
3. 顯示提示：此商店已串接於其他團隊
   * 若想重新串接 SHOPLINE 商店於另一個 Omnichat 團隊，須將 SHOPLINE 商店原有串接解除後再重新進行串接
   * 若是先前從 SHOPLINE 後台進行串接，則須從 SHOPLINE 後台移除擴充功能
   * 若是先前從 Omnichat 後台進行串接，則須從 Omnichat  後台解除串接
4. 顯示提示：此團隊已串接於其他商店
   * 若想重新串接此團隊於另一個 SHOPLINE 商店，須將此團隊原有串接解除後再重新進行串接
   * 若是先前從 SHOPLINE 後台進行串接，則須從 SHOPLINE 後台移除擴充功能
   * 若是先前從 Omnichat 後台進行串接，則須從 Omnichat  後台解除串接

{% hint style="warning" %}
注意：因 SHOPLINE API 有呼叫上限之限制，請盡量避免從 SHOPLINE 後台手動一次<mark style="color:red;">**大量**</mark>貼標或修改資料，以免資料可能無法即時同步過來，及後續場景無法馬上應用。
{% endhint %}
