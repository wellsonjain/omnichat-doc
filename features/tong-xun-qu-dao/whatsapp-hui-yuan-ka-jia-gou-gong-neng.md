---
description: >-
  透過會員卡功能，可讓 WhatsApp 聯絡人主動在 WhatsApp 官方帳號中，自行查詢官網會員資料，加強整合電商平台與您的 WhatsApp
  在會員資訊上的資訊設定
---

# WhatsApp 會員卡設定（加購功能）



{% hint style="info" %}
1. 目前該功能僅限自架官網的品牌使用。若不是自架網站者，後續 Omnichat 會持續優化相關功能，敬請期待
2. 若想查詢 LINE 會員卡功能，請參考 [**LINE 會員卡設定**](https://app.gitbook.com/o/-L_qBouk_wijumBR7PT3/s/-LaFmilpuDQ-f7VKjHCH/~/changes/1610/features/tong-xun-qu-dao/line-hui-yuan-ka-she-ding-jia-gou-gong-neng)
{% endhint %}

## 後台設定畫面（品牌方畫面）

### 1 會員卡設定 <a href="#whatsapp-membercard-setting" id="whatsapp-membercard-setting"></a>

* 會員卡設定頁面路徑： 通訊渠道> 會員卡設定
* 選擇 WhatsApp 頁籤，並點選紅框中的鉛筆圖示開始進行編輯

<figure><img src="../../.gitbook/assets/image (385).png" alt=""><figcaption></figcaption></figure>

### 1-1 會員卡顯示條件

<figure><img src="../../.gitbook/assets/截圖 2024-05-24 下午2.55.02.png" alt=""><figcaption></figcaption></figure>

若目前自架網站的會員號碼有同步至 Omnichat 系統，建議開啟 “在Omnichat 中具備會員編號” 並完成相關設定。此設定能提醒及引導非會員至官網完成會員註冊

1. 查無會員訊息：設計查無會員時所顯示的訊息
2. 按鈕文案：設計引導訪客至官網註冊會員的文案
3. 按鈕連結：貼上引導訪客至官網註冊會員的連結



<figure><img src="../../.gitbook/assets/截圖 2024-05-24 下午4.45.26.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
若關閉 “在 Omnichat 中具備會員編號“，則顧客點選會員卡連結時，一律會顯示會員卡畫面，若無資料則會顯示 “-”
{% endhint %}



### 1-2 會員中心可設定的欄位

<figure><img src="../../.gitbook/assets/截圖 2024-05-24 下午3.26.48.png" alt=""><figcaption></figcaption></figure>

* 若開啟會員中心，可設定以下資訊：

1. 會員條碼：支援以下條碼
   * Code128
   * Code39
   * EAN-13
   * QR Code
2. 顯示資訊：自訂顯示欄位資訊及在會員卡上要顯示的欄位名稱
   * 支援的顯示資訊包含：
     * 顧客姓名
     * 會員編號
     * 電話
     * Email
     * 累積點數 (須購買點數功能)
     * 點數餘額 (須購買點數功能)
     * 自訂屬性 (須購買自訂屬性功能)
   * 紅框內的圖示為自訂顯示欄位順序功能

{% hint style="info" %}
請留意自定顯示欄位沒有上限，但不可重覆設定
{% endhint %}

### 1-3 會員卡標題 icon 設定 <a href="#whatsapp-membercard-uisetting" id="whatsapp-membercard-uisetting"></a>

在會員中心的顯示資訊中，可開啟「顯示 icon」的設定。

<figure><img src="../../.gitbook/assets/截圖 2024-11-04 下午12.04.36.png" alt=""><figcaption></figcaption></figure>

1. 在會員中心的顯示資訊中，可開啟 「 顯示 icon 」 的設定。
2. 開啟後，每個顯示資訊都有預設 icon，也可再上傳指定 icon，格式如下：
   * 建議使用 png 檔
   * 尺寸長寬比 1:1
   * 大小低於 1MB
   * 上傳 icon 後，可點選 「 回預設 」 改為預設 icon 圖示
3. 設定並上傳icon後，可以在右側的預覽畫面查看。

### 1-4 會員卡-外觀設定 <a href="#whatsapp-membercard-uisetting" id="whatsapp-membercard-uisetting"></a>

<figure><img src="../../.gitbook/assets/截圖 2024-05-24 下午4.28.04.png" alt=""><figcaption></figcaption></figure>

* 外觀設定可設定會員卡畫面是否要顯示上方圖示
* 若沒有上傳圖片，則會員卡畫面則不會出現此圖示區塊
* 上傳圖片的建議尺寸為：**1200 \* 512 px**，會等比例自動縮放圖片大小，若比例不等處會留白

### 會員卡使用方法 <a href="#whatsapp-membercard-useway" id="whatsapp-membercard-useway"></a>

<figure><img src="../../.gitbook/assets/截圖 2024-05-24 下午3.50.17.png" alt=""><figcaption></figcaption></figure>

完成設定並啟用後，可透過以上方式將會員卡連結並提供給聯絡人進行會員資訊查閱：

1. 在自助設計機器人中使用系統預設模組 「會員中心」 （左方截圖）
   * 設定方式：在自助設計機器人 中 > 新增 WhatsApp 機器人 > 新增「文字訊息」卡片 > 點擊按鈕名稱 > 回覆對話模組下拉選擇系統預設模組「會員中心」
2. 利用 WhatsApp 訊息範本的快速回覆，按鈕動作選擇會員中卡片（右方截圖）
   * 關於設定WhatsApp 訊息範本，[請參考](https://docs.omnichat.ai/features/tong-xun-qu-dao/integrations/whatsapp-business-api-zheng-he-dao-omnichat/chuang-jian-whatsapp-fan-ben-xun-xi)

## 會員中心（顧客端顯示畫面） <a href="#whatsapp-membercard-membercenter" id="whatsapp-membercard-membercenter"></a>

<figure><img src="../../.gitbook/assets/截圖 2024-05-24 下午4.29.31.png" alt=""><figcaption></figcaption></figure>

1. 使用系統預設模組 「會員中心」 所顯示的 WhatsApp 會員卡訊息畫面
2. 點選會員中心機器人按鈕後，會彈出"開啟會員中心"的卡片。點選此按鈕便可進入會員中查看會員資訊。此連結屬動態會員卡連結，僅有效30分鐘。連結過期後需重新觸發會員中卡片

<figure><img src="https://lh7-us.googleusercontent.com/X78frq2OUqnTWOcPGxxziYfYK_PcGmD8gUJ-V6AHilXjP3LUjc-GedNXNBlo283gvoPQg-wyShSPYmEG-ezi6WvlDlm_oubV9gKPqt7tgFZPdYKdC1Yjj3oQYGDqYNRpU8JGGh2Bckaz1jL-JiVlLAVL3g=s2048" alt="" width="375"><figcaption></figcaption></figure>

{% hint style="warning" %}
&#x20;超過 30 分鐘有效期限點撃會員中心按鈕將出現以上畫面
{% endhint %}

## 其他常見問題（顧客端顯示畫面） <a href="#whatsapp-membercard-qa" id="whatsapp-membercard-qa"></a>

{% hint style="danger" %}
若顧客端顯示以下錯誤資訊，代表目前 WhatsApp 會員卡功能狀態為 「已停用」。請品牌端確認是否需要重新開啟
{% endhint %}

<figure><img src="https://lh7-us.googleusercontent.com/IJ-SUGuGsm0w5FsJAkIp1aSVMAIoj1UDJtahfJyQu6dVoltqj09yPB3uQPHJTZiWUuE5oMTgnGNCXbJGxkGJPeJa_DYWA62Mr_1u8iN025e1NOtJGPENrLTJjpk4ac9RnCvKbFhwG-gR8TAIMjE_bLGN8Q=s2048" alt="" width="375"><figcaption></figcaption></figure>

\
