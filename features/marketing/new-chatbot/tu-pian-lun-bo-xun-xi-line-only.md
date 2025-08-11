---
description: 適用平台：LINE
---

# 圖片輪播訊息 (LINE only)

## 呈現範例

使用情境為希望一次向客戶傳送多張圖片訊息，並在客戶點擊圖片/按鈕後，可前往另一網頁或下一個模組。

<div align="left"><figure><img src="../../../.gitbook/assets/圖片輪播訊息卡片範例1" alt="" width="300"><figcaption><p>按鈕呈現動態範例</p></figcaption></figure></div>

## 預覽文字

訊息卡片支援文字、連結、Emoji、替換變數。

<div align="left"><figure><img src="../../../.gitbook/assets/截圖 2025-03-13 下午3.48.55 (1).png" alt=""><figcaption><p>圖片輪播訊息卡片</p></figcaption></figure></div>



{% hint style="info" %}
文字限制：最多 400 字，一個中文字為一個字
{% endhint %}

圖片長度最多為寬度的3倍、檔案上限 1 MB、適用格式 「.jpg, .jpeg, .png」

## **點擊圖片動作**

1. **回覆模組：**&#x7576;客人按下圖片時，會前往對應的對話模組。
2. **開啟URL：**&#x7576;客戶按下圖片時，會打開瀏覽器前往該URL。

{% hint style="info" %}
**開啟URL:** 右下角支援替換參數。
{% endhint %}

<div align="left"><figure><img src="../../../.gitbook/assets/截圖 2025-03-13 下午3.59.18.png" alt="" width="383"><figcaption><p>右下角支援替換參數，惟網站對話插件平台不支援此功能</p></figcaption></figure></div>

## **點擊按紐動作**

1. **回覆模組：**&#x7576;客人按下按鈕時，會前往對應的對話模組。
2. **開啟URL：**&#x7576;客戶按下按鈕時，會打開瀏覽器前往該URL。

<div align="left"><figure><img src="../../../.gitbook/assets/image (480).png" alt="" width="334"><figcaption><p>按鈕設定詳情</p></figcaption></figure></div>

按鈕名稱：最多 20 個字，一個中文字都算一個字。

按鈕文字顏色：預設為 「黑色」，也可另選 「白色」。

按鈕背景顏色：預設為 「白色」，點選後出現系統預設調色盤可改顏色。

{% hint style="success" %}
**向LINE 好友分享機器人訊息：**

您現在可以使用 **Chatbot 2.0** 設定動作，讓顧客能將聊天機器人的訊息分享給他們的 LINE 好友。此功能**僅支援 LINE 平台**，且**僅適用於 Chatbot 2.0**

<img src="../../../.gitbook/assets/image (511).png" alt="" data-size="original">

1. **支援卡片與按鈕類型**\
   以下卡片按鈕可以支援設定此點擊觸發動作「分享給 LINE 好友」\

   * 文字訊息 (包含真人客服卡片)
     * 一般按鈕
   * 輪播訊息
     * 點擊圖片動作
     * 一般按鈕
   * 圖片輪播訊息
     * 點擊圖片動作
     * 一般按鈕
2. **限制**
   1. 以下是可以被分享出去的卡片類型：
      * 文字訊息
      * 圖像訊息
      * 輪播訊息
      * 圖片輪播訊息
      * 圖文訊息
      * 影片
   2. 被分享出去的卡片中，卡片按鈕限制如下：
      * 僅允許使用 「URL 類型」 的按鈕動作，例如：
        * 開啟網址
        * 分享給 LINE 好友
      * 若使用其他類型的動作，將會出現錯誤。
      * 若該區塊包含 LINE 圖文選單，則**不能**使用透明背景。
{% endhint %}

## **附加動作**

1. **貼上標籤：**&#x7576;客人按下按鈕時，會自動為該名客人貼上標籤。
2. **存為自訂屬性（加購功能）：**&#x7576;客人按下按鈕時，會自動為該名客人貼上自訂屬性，作為會員資料平台的顧客資料。

#### 新增圖片輪播卡片

往右滑可新增圖片輪播卡片，最多可新增至10張卡片。

<figure><img src="../../../.gitbook/assets/截圖 2025-08-01 下午3.43.22.png" alt=""><figcaption></figcaption></figure>

#### 調整圖片輪播卡片順序

1. 點右側的編輯模組區塊右側邊，並往左拖曳，即可將編輯模組的區塊放大。
2. 點擊要調整順序的卡片，並往想要的方向拖曳，即可調整卡片的順序。

<figure><img src="../../../.gitbook/assets/Adobe Express - 圖片輪播換順序.gif" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
#### 常見問題：為什麼我設定的標題沒有出現在推播內容裡？

您設定的「標題」是屬於圖片輪播訊息中的預覽文字，這段文字只會出現在客人收到的新訊息通知以及LINE訊息預覽列表中，不會出現在實際的推播訊息內容裡。

如果您希望讓客人在推播內容中看到標題，建議可以在輪播訊息前方加上一則文字訊息卡片來呈現。



在推播內容中，圖片輪播訊息前後是否有加入其他卡片，會影響推播後客人看到的訊息預覽，以下是常見的幾種情境：

1. 若推播內容僅有圖片輪播訊息，推播後客人的手機信訊息通知和訊息列表會顯示圖片輪播訊息中的預覽文字。
2. 若有在圖片輪播訊息**前**加上其他卡片，推播後客人手機的新訊息通知會顯示第一張卡片的文字內容，訊息列表會顯示圖片輪播訊息中的預覽文字。
3. 若有在圖片輪播訊息**後**加上其他卡片，推播後客人手機的新訊息通知會顯示圖片輪播訊息中的預覽文字，訊息列表會顯示最後一則卡片的文字內容。
4. 若有在圖片輪播訊息**前**、**後**都加上其他卡片，推播後客人手機的新訊息通知會顯示第一張卡片的文字內容，訊息列表會顯示最後一則卡片的文字內容。
{% endhint %}

1. 僅有圖片輪播訊息的設定，推播後實際呈現範例：

<figure><img src="../../../.gitbook/assets/Screenshot 2025-07-08 at 7.21.43 PM.png" alt=""><figcaption></figcaption></figure>

2. 圖片輪播訊息**前**加上文字訊息卡片，推播後實際呈現範例：

<figure><img src="../../../.gitbook/assets/Screenshot 2025-07-09 at 11.54.51 AM.png" alt=""><figcaption></figcaption></figure>

3. 圖片輪播訊息**後**加上文字訊息卡片，推播後實際呈現範例：

<figure><img src="../../../.gitbook/assets/Screenshot 2025-07-09 at 11.58.00 AM.png" alt=""><figcaption></figcaption></figure>

4. 圖片輪播訊息**前**、**後**加上文字訊息卡片，推播後實際呈現範例：

<figure><img src="../../../.gitbook/assets/Screenshot 2025-07-09 at 11.52.00 AM.png" alt=""><figcaption></figcaption></figure>
