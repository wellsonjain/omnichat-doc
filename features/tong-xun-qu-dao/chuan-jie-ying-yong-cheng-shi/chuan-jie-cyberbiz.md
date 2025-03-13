---
description: 完成與 CYBERBIZ 的串接後，可以將客人的會員資料透過 「自訂屬性」 的格式儲存在 Omnichat 中使用
---

# 串接 CYBERBIZ

{% hint style="info" %}
相關自訂屬性定義請洽詢 「CYBERBIZ」
{% endhint %}

串接 CYBERBIZ 的途徑總共有兩種，請根據您的狀況擇一串接即可\
途徑一：[API Secret 串接](chuan-jie-cyberbiz.md#chuan-jie-tu-jing-yi-api-secret-chuan-jie)\
途徑二：[擴充服務市集串接](chuan-jie-cyberbiz.md#chuan-jie-tu-jing-er-kuo-chong-fu-wu-shi-ji-chuan-jie)

### 串接途徑一：API Secret 串接

若要使用該方式串接，需滿足以下方案條件

Omnichat 方案要求：

* 需加購 CRM 會員模組

CYBERBIZ 方案：

* 您的 CYBERBIZ 方案需為企業版或任一加購抽成方案，且需向 CYBERBIZ 購買 API
* 需要 CYBERBIZ 開通 Webhook 權限並取得 Webhook secret

### 步驟一

前往 Omnichat  「通訊渠道 > 串接應用程式」 頁面，找到CYBERBIZ 的欄位並點擊 「串接」 後，再點擊 「開始」

{% hint style="warning" %}
* 若尚未與 CYBERBIZ 購買 API secret，請使用 途徑二 串接，並先與 CYBERBIZ 聯繫付費使用
* 若已購買 CYBERBIZ App Store 串接版本，請改用 途徑二 串接
{% endhint %}



<figure><img src="../../../.gitbook/assets/截圖 2024-03-20 下午6.31.07.png" alt="" width="375"><figcaption></figcaption></figure>

### 步驟二

填寫 CYBERBIZ 提供的 API username、API secret、Webhook secret 並綁定 LINE 綁定渠道

{% hint style="info" %}
在此設定的 LINE 綁定渠道的 「LINE 官方帳號」 須與 CYBERBIZ 後台 LINE 註冊及登入的 「LINE 官方帳號」相同，才可成功在 Omnichat 綁定會員及 LINE 渠道身份
{% endhint %}



<figure><img src="../../../.gitbook/assets/截圖 2024-03-20 下午6.32.50.png" alt="" width="375"><figcaption></figcaption></figure>

### 步驟三

串接成功後，請先點擊 「複製 Webhook 連結」，下一步會到 CYBERBIZ 後台進行

<figure><img src="../../../.gitbook/assets/截圖 2024-03-20 下午6.37.00.png" alt=""><figcaption></figcaption></figure>

到 CYBERBIZ 後台，找到 「管理中心 > Webhook 設定」 中進行 Webhook 設定如下：

複製 Omnichat Webhook URL 並新增以下  Webhook 事件設定

* 會員註冊
* 會員更新
* 會員 VIP 等級

<figure><img src="../../../.gitbook/assets/截圖 2024-03-21 上午10.07.44.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/截圖 2024-03-21 上午10.08.57.png" alt=""><figcaption></figcaption></figure>

### 步驟四

回到 Omnichat 點擊下一步，完成 CYBERBIZ 串接後，即可前往自訂屬性查看同步的會員資料，\
後續再視您是否有購買會員卡模組，可繼續前往設定手機綁定、會員卡。

<figure><img src="../../../.gitbook/assets/截圖 2024-03-21 上午10.12.07.png" alt=""><figcaption></figcaption></figure>



### 串接途徑二：擴充服務市集串接

若要使用該方式串接，需滿足以下方案條件

Omnichat 方案要求：

* 需加購 CRM 會員模組

CYBERBIZ 方案：

* &#x20;您的 CYBERBIZ 方案需為企業版或抽成方案才可使用 (詳情請詢問 CYBERBIZ 服務人員)

### 步驟一

從 CYBERBIZ 後台的擴充服務市集，找到 「Omnichat 全通路會員模組」 的頁面，並點擊 「安裝應用程式」

<figure><img src="../../../.gitbook/assets/截圖 2024-03-20 下午5.44.31.png" alt=""><figcaption></figcaption></figure>

### 步驟二

按照步驟進行：輸入網站 Domain ⮕ 登入商店後台 ⮕ 登入後跳轉至 Omnichat 頁面

<figure><img src="../../../.gitbook/assets/截圖 2024-03-20 下午5.49.06.png" alt="" width="563"><figcaption></figcaption></figure>

### 步驟三

請您登入已經完成購買 CRM 模組的 Omnichat 帳號後台，確認團隊名稱沒問題後，使用管理員帳號進行串接

<figure><img src="../../../.gitbook/assets/截圖 2024-03-19 下午5.27.03.png" alt="" width="295"><figcaption></figcaption></figure>

### 步驟四

同意條款並安裝及授權

<figure><img src="../../../.gitbook/assets/截圖 2024-03-20 下午5.50.54.png" alt="" width="563"><figcaption></figcaption></figure>

### 步驟五

選擇要同步會員資料的 LINE 官方帳號

{% hint style="info" %}
在此設定的 LINE 綁定渠道的 「LINE 官方帳號」 須與 CYBERBIZ 後台 LINE 註冊及登入的 「LINE 官方帳號」相同，才可成功在 Omnichat 綁定會員及 LINE 渠道身份
{% endhint %}

<figure><img src="../../../.gitbook/assets/截圖 2024-03-20 下午5.52.21.png" alt="" width="563"><figcaption></figcaption></figure>

### 步驟六

完成 LINE 官方帳號設定後，會彈出 「已成功編輯資料」 的提醒，便可以進行首次 「同步資訊」，同步後會將目前有使用 LINE 快速登入以及有手機號碼的會員資料同步到對應客人的 LINE 事件上

完成 CYBERBIZ 串接後，即可前往自訂屬性查看同步的會員資料。\
後續再視您是否有購買會員卡模組，可繼續前往設定手機綁定、會員卡。

<figure><img src="../../../.gitbook/assets/截圖 2024-03-21 上午10.12.07.png" alt="" width="457"><figcaption></figcaption></figure>



### 注意事項

若您在串接過程中遇到問題，請根據顯示的提示內容進行排查，以下提供相關提示的介紹

1. 顯示提示：尚未購買 CRM 模組
   * 欲串接團隊尚未購買 CRM 模組，則無法成功串接，需與客服聯繫獲得進一步協助
   * 若選擇錯誤團隊則請重新登入選擇其他團隊串接
2.  顯示提示：此帳號無串接權限

    若登入的帳號非主管或管理員，則無法進行串接功能，請重新登入有權限的帳號以利串接
3. 顯示提示：此商店已串接於其他團隊
   * 若想重新串接 CYBERBIZ 商店於另一個 Omnichat 團隊，須將 CYBERBIZ 商店原有串接解除後再重新進行串接
   * 若是先前從 CYBERBIZ 後台進行串接，則須從 CYBERBIZ 後台移除擴充功能
   * 若是先前從 Omnichat 後台進行串接，則須從 Omnichat  後台解除串接
4. 顯示提示：此團隊已串接於其他商店
   * 若想重新串接此團隊於另一個 Cyberbiz 商店，須將此團隊原有串接解除後再重新進行串接
   * 若是先前從 CYBERBIZ 後台進行串接，則須從 CYBERBIZ 後台移除擴充功能
   * 若是先前從 Omnichat 後台進行串接，則須從 Omnichat  後台解除串接
