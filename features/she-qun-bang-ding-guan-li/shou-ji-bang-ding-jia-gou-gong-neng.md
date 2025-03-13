---
description: 透過 「手機綁定」 功能，可讓顧客於 LINE 上查看個人會員卡資訊。
---

# 手機綁定（加購功能）

{% hint style="info" %}
**使用 「CRM模組、手機綁定」 前重要提醒：**

1、客人<mark style="color:red;">必須先完成</mark>品牌官方網站的<mark style="color:red;">會員註冊</mark>

2、客人在進行手機綁定時，輸入的<mark style="color:red;">手機號碼必須為註冊</mark>品牌網站<mark style="color:red;">會員時的電話號碼</mark>

3、客人在 LINE 首次使用會員卡時，需先完成 「<mark style="color:red;">手機綁定</mark>」 流程才能成功查看。

4、該功能目前僅支援品牌官方網站為： SHOPLINE、Cyberbiz 方能使用，其他開店平台系統商（包含自架網站），後續會再上線相關功能，敬請期待
{% endhint %}

{% hint style="info" %}
「手機綁定」 將會發送 OTP 簡訊傳送驗證碼，正式使用前<mark style="color:blue;">**須先完成簡訊費儲值**</mark>。

詳情可與顧問專員進行聯繫。
{% endhint %}

## 手機綁定前置作業

### SHOPLINE 前置作業

<div align="center"><figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午5.23.04.png" alt=""><figcaption><p>將 SHOPLINE 電商後台 「顧客驗證方式」 - 「手機驗證」 設為 「發送簡訊驗證手機」</p></figcaption></figure></div>

* 前往 SHOPLINE 後台 > 設定 > 顧客設定
* 將顧客註冊方式設為 「僅以手機號碼註冊」  or  「手機號碼與電郵註冊」
* 將顧客驗證方式的手機驗證改為 「發送簡訊驗證手機」

### CYBERBIZ 前置作業

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午5.24.27.png" alt=""><figcaption><p>CYBERBIZ 電商後台 「顧客註冊欄位設定」 - 「手機」 欄位設為 “<strong>必填且需驗證”</strong></p></figcaption></figure>

* 前往 CYBERBIZ 後台 > 管理中心> 顧客註冊設定&#x20;
* 將顧客註冊欄位設定的手機欄位設為必填，並開啟驗證及開啟註冊時驗證電話

### LINE LIFF 設定

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午5.26.31.png" alt=""><figcaption><p>LINE Developers 後台 - Providers - Admin - LINE Login</p></figcaption></figure>

* 使用前需先至 [LINE 後台](https://developers.line.biz/en/) 設定
* 請選擇 LINE Login 的選項\
  （請確保 LINE Login Channel 與 Messaging API Channel 在同一 Providers-Admin 之中）
* 選擇 LIFF 設定
* 請選擇 LIFF app name 為 「社群身份綁定」 的選項進行編輯，若尚未設定，請參照 [教學手冊](https://docs.omnichat.ai/features/tong-xun-qu-dao/integrations/line-2.0/she-qun-shen-fen-bang-ding-liff-she-ding) 先建立完成

<figure><img src="../../.gitbook/assets/image (95).png" alt=""><figcaption><p>LINE Login Channel - LIFF</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午5.28.42.png" alt=""><figcaption><p>LINE Login Channel - LIFF - Endpoint URL</p></figcaption></figure>

* 找到 Endpoint URL，將 URL 中的 「app」 改為 「pages」
* 範例：\
  原網址： https://app.omnichat.ai/liff-bind.html?liffId=1661242192-OQejBARg\
  調整為： https://<mark style="color:red;">pages</mark>.omnichat.ai/liff-bind.html?liffId=1661242192-OQejBARg
* 將 <mark style="background-color:purple;">LIFF Size 設定為 「</mark><mark style="background-color:purple;">**Full**</mark><mark style="background-color:purple;">」</mark>

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午5.30.25.png" alt=""><figcaption><p>設定 Omnichat 後台 「綁定 Liff ID」</p></figcaption></figure>

* 返回 Omnichat 後台（若曾因社群身份綁定，綁定 LIFF ID 已設定過，則不需再設定一次）
* 前往 通訊渠道 > 串接社群通訊渠道，點選 「LINE」 平台，選擇要使用手機綁定的渠道，點選此渠道動作裡的編輯按鈕，更新 「**綁定 Liff ID**」 並按儲存。

## 手機綁定 - 「品牌端」 設定

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午5.35.39.png" alt=""><figcaption><p>手機綁定 - 功能說明</p></figcaption></figure>

* 位於 社群綁定管理 > **手機綁定** 頁面
* **支援 LINE 渠道**
* 若有串接 SHOPLINE / CYBERBIZ 電商平台，手機綁定完成後即可綁定此 **會員編號** 及**LINE** **UID** 身分
* 此設置僅支援，後台管理權限：「管理員、主管」 來操作。
* 設定方式

1. <mark style="color:green;">可於 LINE 自助設計機器人中卡片按鈕設定系統預設模組 > 手機綁定</mark>&#x20;
2. <mark style="color:green;">可取得綁定連結 (動作 > 複製綁定連結) 設定於圖文選單、圖文訊息、機器人模組、1：1 訊息</mark>

* 若有使用會員卡功能，建議直接在機器人或圖文選單中設定 **會員卡** 的綁定連結，但顧客尚未完成手機綁定，點選會員卡的連結後，會引導進行手機綁定流程
* 每個手機綁定渠道皆可設置-暫時停用

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午5.36.02.png" alt=""><figcaption><p>手機綁定 - 設定說明</p></figcaption></figure>

* 每個渠道皆可有不同的手機綁定訊息設定，並可分別針對三種綁定情境選擇發送不同的**文字訊息** 或是 **機器人卡片**，

包含：

* [x] 首次完成綁定訊息
  * 從未綁定過手機完成綁定時
* [x] 已綁定訊息
  * 已綁定過手機，再次點擊綁定連結時
*   [x] 綁定失敗訊息

    * 輸入手機查無對應會員時


* [x] 綁定畫面顯示圖片
  * 預設為團隊大頭貼
  * 可另外上傳尺寸為 1200\*640 大小的圖片

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午5.37.01 (1).png" alt=""><figcaption><p>手機綁定 - 觸發訊息說明</p></figcaption></figure>

* 觸發訊息：系統代替顧客發送的訊息文字，最多60字。
* 用來觸發文字訊息或是機器人卡片。
* 顧客觸發的綁定成功訊息、已綁定訊息、綁定失敗訊息 **皆不收費**。

#### 會員身份比對平台

* 當客人進行手機綁定時，會與所選擇的平台進行比對，檢查該手機號碼是否在官網存在會員編號。如果找不到會員編號，則會發出綁定失敗的訊息
* 可選擇「SHOPLINE」、「Cyberbiz」 or 「不需比對」
* 若是選擇「不需比對」，那麼會檢查此手機號碼是否存在於 Omnichat 系統\
  1.**「若在 Omnichat 系統有找到手機號碼」**，則會將這名 LINE 好友與手機號碼找到的顧客進行合併\
  2.**「若在 Omnichat 系統沒有找到手機號碼」**，則只會將手機號碼更新到這名 LINE 好友身上

#### 首次綁定完成訊息，支援「綁定完成後貼上標籤」

<figure><img src="../../.gitbook/assets/截圖 2024-10-15 下午1.33.43.png" alt=""><figcaption></figcaption></figure>

* 可一次貼上多個標籤
* 當客人被貼上標籤後，可觸發以下兩種情境\
  1.支援觸發顧客旅程\
  2.支援依照標籤切換圖文選單
* 若是已完成手機綁定的客人再次完成手機綁定，不支援再次貼標
* 若需解除綁定，可至[社群聯絡人](../she-qun-ke-hu-zi-liao-ping-tai/she-qun-lian-luo-ren.md)

## 手機綁定 - 「顧客端」 畫面

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午5.39.04.png" alt=""><figcaption><p>手機綁定 - 顧客端流程</p></figcaption></figure>

* **綁定連結**、**綁定卡片** 可透過 <mark style="color:blue;">機器人模組</mark>、<mark style="color:blue;">圖文選單</mark>、<mark style="color:blue;">推播</mark>、<mark style="color:blue;">1：1對話</mark>發送給客戶來完成綁定。
* 暫時不支援 LINE 電腦版。
* 需事先完成 Liff ID 設定。
* 可自定義綁定顯示圖片。

<figure><img src="../../.gitbook/assets/截圖 2024-07-30 下午5.40.41.png" alt=""><figcaption><p>手機綁定 - 顧客端流程</p></figcaption></figure>

### 注意事項：

* 如客戶輸入的手機不是註冊品牌網站會員資料的手機時，會出現查無手機的提示訊息，並發送「**綁定失敗**」 的卡片。
* 如綁定連結是 「**停用中**」 的狀態，客戶開啟連結時會出現 「**綁定連結暫時無法使用**」 的提示需訊息。
