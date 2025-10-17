---
description: 以 Member ID 為唯一識別值來匯入會員基本資料
---

# 匯入顧客名單

## 第一步：匯入檔案

1. 左欄 「 渠道客戶資料平台 」 > 「 資料匯入 」 > 點選右上角的 「 匯入 」

<figure><img src="../../../.gitbook/assets/截圖 2025-10-03 下午4.33.10 (1).png" alt=""><figcaption></figcaption></figure>

2. 選擇 「 匯入顧客 」

<figure><img src="../../../.gitbook/assets/截圖 2025-10-03 下午4.52.33拷貝.png" alt="" width="563"><figcaption></figcaption></figure>

3. 依照標籤匯入方式下載範例檔案

<figure><img src="../../../.gitbook/assets/截圖 2025-10-05 上午11.34.11.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
* CSV 檔案如非為 UTF-8 encoding 版本會呈現亂碼，為避免版本問題，建議您使用 [**Google Sheet**](https://docs.google.com/spreadsheets/) 進行操作。
* **上傳檔案時須留意：**<mark style="color:red;">**勾選「覆蓋標籤」會移除聯絡人原有的所有標籤，並新增匯入的標籤。**</mark>
{% endhint %}

### **如何編輯CSV檔案？CSV檔案注意事項**

* <mark style="color:red;">**Member ID為必填欄位。**</mark>

<figure><img src="../../../.gitbook/assets/image (415).png" alt="" width="563"><figcaption><p>檔案中一定要填寫Member ID</p></figcaption></figure>

* 電話號碼須為國際格式：
  * 請移除號碼開頭的「0」或特殊撥號
  * 例如：
    * 臺灣手機 0911223344，請輸入 <mark style="color:red;">**886**</mark>911223344；
    * 香港手機 91122333，請輸入 <mark style="color:red;">**852**</mark>91122333；
    * 新加坡手機 81234567，請輸入 <mark style="color:red;">**65**</mark>81234567；
    * 馬來西亞手機 123456789，請輸入 <mark style="color:red;">**60**</mark>123456789
  * 若使用 Excel 編輯 CSV 文件時，電話需先轉成<mark style="color:red;">**文字格式**</mark>，以避免位數過長轉換成科學記號
* 匯入資料時，若 "Email"、"Phone" 欄位有重複，全渠道顧客資料可能會互相覆蓋

### **如何匯入顧客的自訂屬性？**

<div align="center"><figure><img src="../../../.gitbook/assets/image (329).png" alt="" width="428"><figcaption></figcaption></figure></div>

{% hint style="info" %}
* 檔案建議小於30MB，超過請分批匯入
* 支援非同步匯入，上傳檔案後，可離開頁面等匯入完成
* 在匯入進行中時，您仍可以上傳其他檔案，並等待排程處理。
{% endhint %}

## 第二步：資料對應

1. 將編輯好的CSV檔案拖拉，或者選擇檔案至上傳檔案區，再按下一步

<figure><img src="../../../.gitbook/assets/截圖 2025-10-05 上午11.34.11 (1).png" alt=""><figcaption></figcaption></figure>

2. 選擇對應的系統資料（通常維持預設即可）

<figure><img src="../../../.gitbook/assets/截圖 2025-10-05 上午11.34.31.png" alt=""><figcaption></figcaption></figure>

## 第三步：資料驗證

1. 系統進行資料驗證後，如有錯誤資訊則會跳提醒，請求重新上傳檔案

<figure><img src="../../../.gitbook/assets/截圖 2025-10-03 下午4.38.46拷貝.png" alt=""><figcaption></figcaption></figure>

2. 如果資料正確，即可點選右上角的匯入

<figure><img src="../../../.gitbook/assets/截圖 2025-10-03 下午4.38.57 (1).png" alt=""><figcaption></figcaption></figure>

3. 資料匯入過程中，若您想要取消匯入，可以在此時取消

<figure><img src="../../../.gitbook/assets/截圖 2025-10-05 上午11.40.22.png" alt=""><figcaption></figcaption></figure>

4. 您也可以回到列表等待排程，若狀態為 「 等待中 」，可點選動作來取消匯入

<figure><img src="../../../.gitbook/assets/截圖 2025-10-03 下午4.39.28拷貝 (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/截圖 2025-10-03 下午4.39.36拷貝 (1).png" alt=""><figcaption></figcaption></figure>

5. 以下為匯入前 及 成功匯入後 顧客資料：

<figure><img src="../../../.gitbook/assets/image (341).png" alt=""><figcaption><p>匯入前顧客資料</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (342).png" alt=""><figcaption><p>成功匯入後顧客資料</p></figcaption></figure>

