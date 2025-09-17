---
description: 以社群 User ID 為唯一識別值來匯入社群名單及會員基本資料；若有購買 OMO 方案，WhatsApp 、LINE 渠道支援匯入此顧客綁定的團隊成員
---

# 匯入社群聯絡人

## 第一步：匯入檔案

**左欄“社群客戶資料平台” > “匯入顧客資料” > 點選右上角的“匯入”**

<figure><img src="../../../.gitbook/assets/image (416).png" alt="" width="563"><figcaption></figcaption></figure>

**選擇“匯入社群聯絡人”**

<figure><img src="../../../.gitbook/assets/匯入社群聯絡人.png" alt="" width="563"><figcaption><p>選擇匯入社群聯絡人</p></figcaption></figure>

先選擇欲匯入的通訊渠道

<figure><img src="../../../.gitbook/assets/選擇渠道.png" alt="" width="563"><figcaption><p>先選擇渠道</p></figcaption></figure>

**再依照該渠道的標籤匯入方式下載範例檔案**

<figure><img src="../../../.gitbook/assets/社群聯絡人依照標籤匯入方式下載範例檔案.png" alt=""><figcaption><p><strong>依照該渠道的標籤匯入方式下載範例檔案，需留意覆蓋標籤</strong></p></figcaption></figure>

{% hint style="warning" %}
* CSV 檔案如非為 UTF-8 encoding 版本會呈現亂碼，為避免版本問題，建議您使用 [**Google Sheet**](https://docs.google.com/spreadsheets/) 進行操作。
* **上傳檔案時須留意：**<mark style="color:red;">**勾選「覆蓋標籤」會移除聯絡人原有的所有標籤，並新增匯入的標籤。**</mark>
{% endhint %}



**如何編輯CSV檔案？**

* <mark style="color:red;">**各渠道的 User ID為必填欄位，以下以Line為例子。**</mark>

<figure><img src="../../../.gitbook/assets/image (346).png" alt="" width="563"><figcaption><p>以 LINE 作為範例</p></figcaption></figure>

* 電話號碼須為國際格式：
  * 請移除號碼開頭的「0」或特殊撥號
  * 例如：
    * 臺灣手機 0911223344，請輸入 <mark style="color:red;">**886**</mark>911223344；
    * 香港手機 91122333，請輸入 <mark style="color:red;">**852**</mark>91122333；
    * 新加坡手機 81234567，請輸入 <mark style="color:red;">**65**</mark>81234567；
    * 馬來西亞手機 123456789，請輸入 <mark style="color:red;">**60**</mark>123456789
  * 若使用 Excel 編輯 CSV 文件時，電話需先轉成<mark style="color:red;">**文字格式**</mark>，以避免位數過長轉換成科學記號
* 如欲綁定OMO團隊成員須同時填寫 "<mark style="color:blue;">**Binding Teammate**</mark>" 及 "<mark style="color:blue;">**Store Location Code**</mark>"，且只有<mark style="color:blue;">**銷售人員**</mark>或<mark style="color:blue;">**銷售經理**</mark>才能被綁定；如欲解除綁定，請在 "Binding Teammate" 欄位輸入 UNASSIGNED
  * 若需要匯入顧客資料到綁定 OMO 銷售人員或銷售經理，請在 <mark style="color:blue;">**Store Location Code**</mark> 該欄位當中，填入銷售人員或銷售經理的<mark style="color:blue;">**分店編號**</mark>

<figure><img src="../../../.gitbook/assets/image (350).png" alt="" width="563"><figcaption><p>OMO綁定成員、分店</p></figcaption></figure>

* 匯入資料時，若 "Email", "Phone" 欄位有重複，全渠道顧客資料可能會互相覆蓋



**如何匯入顧客的自訂屬性？**

<figure><img src="../../../.gitbook/assets/image (347).png" alt="" width="428"><figcaption></figcaption></figure>

{% hint style="info" %}
* 檔案建議小於30MB，超過請分批匯入
* 支援非同步匯入，上傳檔案後，可離開頁面等匯入完成
* 在匯入進行中時，您仍可以上傳其他檔案，並等待排程處理。
{% endhint %}

## 第二步：資料對應

**將編輯好的CSV檔案拖拉，或者選擇檔案至上傳檔案區，再按下一步**

<figure><img src="../../../.gitbook/assets/檔案上傳 (1).png" alt="" width="563"><figcaption><p>上傳檔案後按下一步</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (348).png" alt=""><figcaption><p>系統進行資料對應</p></figcaption></figure>

## 第三步：資料驗證

**系統進行資料驗證後，如有錯誤資訊則會跳提醒，請求重新上傳檔案**

<figure><img src="../../../.gitbook/assets/匯入聯絡人資料錯誤.png" alt=""><figcaption><p>如csv檔有錯誤資料，則系統會跳提醒「重新上傳檔案」</p></figcaption></figure>

**如果資料正確，即可點選右上角的匯入**

<figure><img src="../../../.gitbook/assets/image (351).png" alt=""><figcaption><p>重新上傳檔案後，如資料皆正確，即可進行匯入</p></figcaption></figure>

**資料匯入過程中，若您想要取消匯入，可以在此時取消**

<figure><img src="../../../.gitbook/assets/image (417).png" alt="" width="563"><figcaption><p>資料匯入進度</p></figcaption></figure>

**您也可以回到列表等待排程，若狀態為「等待中」，可點選動作來取消匯入**

<figure><img src="../../../.gitbook/assets/image (418).png" alt="" width="563"><figcaption><p>列表</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (419).png" alt="" width="563"><figcaption><p>點選動作亦可以取消匯入</p></figcaption></figure>

**如果您不打算取消匯入，可繼續等待直至資料匯入完成**

<figure><img src="../../../.gitbook/assets/image (353).png" alt=""><figcaption><p>資料匯入完成</p></figcaption></figure>

**以下為成功匯入後的新顧客資料：**

<figure><img src="../../../.gitbook/assets/image (354).png" alt=""><figcaption><p>成功匯入後顧客資料</p></figcaption></figure>
