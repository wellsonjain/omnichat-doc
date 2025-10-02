---
description: '支援社群渠道: WhatsApp'
---

# WhatsApp Flow 卡片 (WhatsApp only)

**WhatsApp Flows** 是 Meta 推出的功能，可以直接在 WhatsApp 中設計並使用互動表單。這能簡化互動流程，無需跳轉至其他應用程式或網站，整個過程都能在 WhatsApp 內完成。

透過 WhatsApp Flows，您可以設計逐步的互動流程，讓客人能夠：

* 快速分享回饋
* 填寫並提交表單
* 報名活動或優惠
* 發送特定的支援需求給團隊
* 完成問卷調查
* 預約時間
* 登入帳號
* 取得服務資訊，例如價格或條款

除了上述範例，WhatsApp Flows 還提供更多功能，協助企業在 WhatsApp 內直接處理各種客戶互動。

<figure><img src="../../../.gitbook/assets/image (521).png" alt=""><figcaption></figcaption></figure>

接下來將介紹如何設定與管理 WhatsApp Flows，如何將 Flow 連結到機器人模組卡片並發送給客人，以及哪些角色具備管理 Flows 的權限。

* [擁有 WhatsApp Flows 權限的角色](whatsapp-flow-ka-pian-whatsapp-only.md#yong-you-whatsapp-flows-quan-xian-de-jue-se)
* [設定與管理 WhatsApp Flows](whatsapp-flow-ka-pian-whatsapp-only.md#she-ding-yu-guan-li-whatsapp-flows)
  * [步驟 1：建立 WhatsApp Flow 表單](whatsapp-flow-ka-pian-whatsapp-only.md#bu-zhou-1-jian-li-whatsapp-flow-biao-dan)
  * [步驟 2：於 Omnichat 平台查看 Flow 清單](whatsapp-flow-ka-pian-whatsapp-only.md#bu-zhou-2-wu-omnichat-ping-tai-cha-kan-flow-qing-dan)
  * [步驟 3：設定客人回覆Flow後的觸發動作與回應儲存方式](whatsapp-flow-ka-pian-whatsapp-only.md#bu-zhou-3-she-ding-ke-ren-hui-fu-flow-hou-de-chu-fa-dong-zuo-yu-hui-ying-chu-cun-fang-shi)
  * [步驟 4：透過機器人模組或WhatsApp訊息範本分享 Flow](whatsapp-flow-ka-pian-whatsapp-only.md#bu-zhou-4-tou-guo-ji-qi-ren-mo-zu-huo-whatsapp-xun-xi-fan-ben-fen-xiang-flow)
  * [步驟 5：查看或匯出回覆紀錄](whatsapp-flow-ka-pian-whatsapp-only.md#bu-zhou-5-cha-kan-huo-hui-chu-hui-fu-ji-lu)

## 擁有 WhatsApp Flows 權限的角色

<table><thead><tr><th width="144.875">權限角色 / 行動</th><th>查看 Flow</th><th>編輯 Flow</th><th>查看回應紀錄</th><th>匯出紀錄 CSV</th></tr></thead><tbody><tr><td>管理員</td><td>✔️</td><td>✔️</td><td>✔️</td><td>✔️</td></tr><tr><td>主管</td><td>✔️</td><td>✔️</td><td>✔️</td><td>✔️</td></tr><tr><td>行銷人員</td><td>✔️</td><td>✔️</td><td>✔️</td><td>✔️</td></tr><tr><td>客服主管</td><td>✔️</td><td>✔️</td><td>✔️</td><td>✔️</td></tr><tr><td>客服人員</td><td>✔️</td><td>Ｘ</td><td>✔️</td><td>Ｘ</td></tr><tr><td>銷售經理</td><td>Ｘ</td><td>Ｘ</td><td>Ｘ</td><td>Ｘ</td></tr><tr><td>銷售人員</td><td>Ｘ</td><td>Ｘ</td><td>Ｘ</td><td>Ｘ</td></tr><tr><td>行銷客服人員（需加購）</td><td>✔️</td><td>✔️</td><td>✔️</td><td>✔️</td></tr></tbody></table>

## 設定與管理 WhatsApp Flows

### **步驟 1：建立 WhatsApp Flow 表單**

我們的團隊會協助您在 WhatsApp Manager 帳號中建立並客製化 Flow。

{% hint style="info" %}
若您的 WhatsApp Flow 表單包含多個區塊，設定時間會較長，請預留額外工作日。
{% endhint %}

### **步驟 2：於 Omnichat 平台查看 Flow 清單**

在 WhatsApp Manager 發佈 Flow 後，將會同步到 Omnichat 後台：串接通訊渠道 > WhatsApp Flows。您可以設定回覆流程及互動內容。

<figure><img src="../../../.gitbook/assets/截圖 2025-09-16 上午11.10.13.png" alt=""><figcaption></figcaption></figure>

* 清單每小時更新一次（於每小時第 5 分鐘）。
* 清單顯示資訊包含：
  * 名稱：不可重複，最多 200 字元（不會顯示給客戶）
  * Flow ID：用於識別各 Flow
  * 分類：Flow 可屬於多種類型
    * 註冊
    * 登入
    * 預約
    * 獲取潛在客戶
    * 聯絡我們
    * 客服支援
    * 問卷調查
    * 其他
  * 狀態：
    * 草稿：Flow的內容仍可編輯，但不能發送給客人
    * 已發布：Flow的內容不可再次編輯或刪除
    * 已棄用：不可刪除、不可發送，也不可恢復成已發布狀態，即便從已發送出去的訊息中，也無法再次打開Flow
    * 暫停：WhatsApp Flow系統偵測異常，將無法發送與開啟
    * 被限制：WhatsApp Flow系統偵測異常，僅能每小時發送 10 則 Flow
  * 總回應數：紀錄客人有完成 Flow 回應的總數，每個客人只能在同一個 Flow 回應一次。
  * 動作：
    * 編輯：編輯客人回應 Flow 後的觸發動作與其他設定
    * 查看回應紀錄：查看Flow的回應紀錄

根據狀態不同，可以執行的動作也不盡相同，請參考下方表格：

| 草稿  | ✔️ | ✔️ | Ｘ                | Ｘ  |
| --- | -- | -- | ---------------- | -- |
| 已發布 | Ｘ  | Ｘ  | ✔️               | ✔️ |
| 已棄用 | Ｘ  | Ｘ  | Ｘ                | Ｘ  |
| 暫停中 | Ｘ  | Ｘ  | Ｘ                | Ｘ  |
| 被限制 | Ｘ  | Ｘ  | ✔️ (10 per hour) | ✔️ |

### 步驟 3：設定客人回覆Flow後的觸發動作與回應儲存方式

點擊最右側&#x7684;**「動作」**&#x6309;鈕中&#x7684;**「編輯」**&#x9032;行設定。

<figure><img src="../../../.gitbook/assets/截圖 2025-09-16 上午11.13.59.png" alt=""><figcaption></figcaption></figure>

1. **回應後觸發動作**

* **回應成功訊息**：當客人完成Flow後系統會回覆一則預設訊息：「感謝您完成填寫！」，可自行修改並加入 emoji 或名字
* **附加訊息**：預設為「不發送」，可改為文字或機器人模組（僅限 WhatsApp 機器人模組）
* **貼上標籤**：客戶完成Flow後自動貼上標籤

2.  **回應儲存設定**

    可點擊頁面左下角的「選擇欄位」按鈕，選擇要儲存在 Omnichat 的資料，支援自訂屬性或系統預設欄位（如姓名、Email）。

### **步驟 4：**&#x900F;過機器人模組或WhatsApp訊息範本分享 Flow

#### **機器人模組**

Flow 卡片僅限於 WhatsApp 使用，可以編輯的部分有四個區塊包含：

<figure><img src="../../../.gitbook/assets/截圖 2025-09-16 上午11.16.18.png" alt=""><figcaption></figcaption></figure>

1. **標題**
   * **無**
   * **文字**：最多 80 字
   * **媒體**：
     * 圖片：可支援JPG/JPEG/PNG格式，檔案上限為 5MB，若超過 5MB 則會自動壓縮
     * 影片：可支援MP4格式，檔案上限為 10MB
2. **內文**：必填，最多 550 字，可加入 emoji 與變數
3. **頁尾**：選填，最多 60 字，不支援 emoji/變數
4.  **按鈕**：

    <figure><img src="../../../.gitbook/assets/截圖 2025-09-16 上午11.19.02.png" alt=""><figcaption></figcaption></figure>

    * 按鈕名稱：必填，最多 20 字（不支援 emoji）
    * Flow ID：必填，狀態為草稿、已發布、被限制皆可選擇
    * Screen ID：預設為第一個畫面，不能修改
    * 僅能新增一個按鈕

#### WhatsApp 訊息範本

Flow 可透過 CTA 按鈕加入訊息範本中，我們新增了一顆「Flow」的按鈕，當客人點擊後即可開啟 Flow。

<figure><img src="../../../.gitbook/assets/截圖 2025-09-16 上午11.20.47.png" alt=""><figcaption></figcaption></figure>

* 每個訊息範本僅能有一個 Flow 按鈕，且不能跟其他 CTA 按鈕共用。
* Flow CTA按鈕設定
  * **按鈕名稱**：必填，最多 20 字（一個中文字視為 3 字元）
  * **Flow ID**：僅限 已公布 或 被限制 狀態
  * **Screen ID**：預設為第一個畫面，不能修改

可已將訊息範本或機器人模組用於一對一聊天、推播、群發訊息（OMO 方案）、或顧客旅程中。

### **步驟 5：查看或匯出回覆紀錄**

點擊最右側&#x7684;**「動作」**&#x6309;鈕中&#x7684;**「回應紀錄」**&#x9032;入頁面。

<figure><img src="../../../.gitbook/assets/截圖 2025-09-16 上午11.22.18.png" alt=""><figcaption></figcaption></figure>

#### 查看回應紀錄

* **搜尋與篩選**
  * 支援姓名、電話搜尋
  * 支援篩選特定日期區間（區間長度不限）
* **列表顯示欄位**：
  * 姓名：客人在 WhatsApp 上的姓名
  * 電話：客人的 WhatsApp 電話號碼
  * 回應時間：客人完成 Flow 的時間（時間格式為：yyyy-MM-dd HH:mm:ss）
* **列表顯示排序：**&#x9810;設顯示所有紀錄，並根據客人完成 Flow 的時間，從最新至最舊排列。
* **動作**：
  * 查看回應紀錄
    * Label：表單各項項目，即在WhatsApp管理工具後台中設定的標籤名稱
    * 回應內容：客人填寫的內容
  * 刪除回應紀錄

#### **匯出回應紀錄**

可以先篩選回應時間區間或特定名單後，再點擊頁面右上角「匯出回應紀錄」按鈕，即可依日期或搜尋條件結果匯出 CSV 檔案。

* 若沒有套用任何篩選條件，預設將會匯出所有回應紀錄
* 若有套用篩選條件後，僅匯出符合條件的回覆
* 匯出的 CSV 檔名為 Flow 名稱
* 匯出的 CSV 檔案欄位包含：
  * customer\_name：客人的姓名
  * customer\_phone：客人的電話
  * customer\_response\_time：客人的回應時間
  * Flow 設定的其他欄位

<figure><img src="../../../.gitbook/assets/截圖 2025-09-16 上午11.24.26.png" alt=""><figcaption></figcaption></figure>

部分 Flow 可能要求客戶上傳圖片、影片或檔案：

<figure><img src="../../../.gitbook/assets/image (522).png" alt=""><figcaption></figcaption></figure>

* **回應紀錄頁面直接顯示**：可於 回應紀錄按鈕中直接查看客人上傳的圖片或檔案

<figure><img src="../../../.gitbook/assets/image (524).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (525).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (526).png" alt=""><figcaption></figcaption></figure>

* **匯出紀錄**：支援匯出含有圖片、檔案、影片的 CSV 檔案
*   **Webhook 支援**：

    * 支援第三方廠商透過 Omnichat Webhook 接收客人從 WhatsApp 上完成的 Flow 資料，不需再另外手動從 Omnichat 後台下載資料（此功能需要您的的工程團隊一同協助整合）
    * **設定方式**：可於開發者中心 > Webhook 設定頁面新增 Topic 為「whatsapp\_flow/flow\_create」的觸發事件。
    * **觸發時機**：顧客填寫完 Flow 時，Omnichat 會收到資料並儲存，同時發送事件至你指定的 Endpoint URL。

    <figure><img src="../../../.gitbook/assets/image (523).png" alt=""><figcaption></figcaption></figure>

    * 回應格式：

```
{
   "customer_name": "Ruby",
   "customer_phone": "886900000000",
   "customer_response_time": "2024-07-31T12:00:37.206+08:00",
   "flow_response": {
      "姓名": "王菲菲",
      "公司名稱": "Omnichat科技公司",
      "職位": "業務人員",
      "公司網址": "台北市大安區忠孝東路四段123456號",
      "手提電話": "0900000000",
      "公司電郵": "Omnichat@mail.com",
      "選擇計畫": [
         "預約服務",
         "意見調查",
         "登記促銷",
      ],
      "選擇分數": "★★★★ 有興趣",
      "預約日期": "1732204800000",
      "預約時段": "09:00-12:00",
   },
}
```

更多詳細設定方式，請參考以下文件：

* [WhatsApp Flows Omnichat 使用指南](https://docs.google.com/presentation/d/1qMVpm9qQzBEXsYhuTnwB8HdYDgwr0p1CiZyin6Gsnws/edit#slide=id.g130dd4f43c0_3_150)
* [WhatsApp Flows Meta 官方指南](https://developers.facebook.com/docs/whatsapp/flows/introduction)
