---
description: 支援發送透過 LINE Simulator 設計的各種訊息樣式
hidden: true
---

# LINE Flex Message（加購功能）

## **內容設定**

1. 設定訊息範本名稱、聊天列表的預覽標題
2. 在 [LINE Flex Message Simulator](https://developers.line.biz/flex-simulator) 設計好訊息樣式後，點擊 「 View as JSON 」 並複製

<figure><img src="../../.gitbook/assets/image (50).png" alt=""><figcaption><p>LINE Flex Message Simulator 中複製訊息 JSON 內容</p></figcaption></figure>

3. 將 JSON 內容貼至 LINE Flex Message 的 JSON 內容區塊

## 追蹤設定

### 追蹤訊息開封率

* 設定方式：
  1.  若需追蹤訊息開封率請先開啟此設定\
      ⚠️ 注意：若是在發送該則訊息後才開啟此設定，無法回溯過去已發送訊息的開封成效

      <figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
  2.  請於 LINE FLEX MESSAGE SIMULATOR 訊息中任一位置新增一張圖片

      <figure><img src="../../.gitbook/assets/image (477).png" alt=""><figcaption></figcaption></figure>
  3.  將圖片的 size 欄位設定為：0px&#x20;

      <figure><img src="../../.gitbook/assets/image (478).png" alt=""><figcaption></figcaption></figure>
  4.  將圖片的 URL 設定為任意值&#x20;

      <figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
  5.  複製 JSON 格式填入 「 內容設定 / JSON 內容 」&#x20;

      <figure><img src="../../.gitbook/assets/image (50).png" alt=""><figcaption><p>LINE Flex Message Simulator 中複製訊息 JSON 內容</p></figcaption></figure>
  6.  複製追蹤訊息開封率的追蹤碼，並將JSON 中該圖片 URL 更換為此追蹤碼

      <figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

***

### 追蹤訊息按鈕 / 圖片動作點擊率

設定方式：

1.  若需追蹤訊息按鈕 / 圖片動作點擊請先開啟此設定\
    ⚠️ 注意：若是在發送該則訊息後才開啟此設定，無法回溯過去已發送訊息的點擊成效

    <figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>
2.  將想要追蹤的按鈕或圖片連結複製並填入下方 URL 區塊中，若有多個按鈕需要追蹤依序透過「新增 URL」 按鈕新增

    <figure><img src="../../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
3.  複製追蹤碼後，將對應的 URL 替換成追蹤碼

    <figure><img src="../../.gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>


4. 特殊情境：若需要追蹤點擊的按鈕或圖片連結有包含品牌自訂變數、Omnichat 系統屬性變數、自訂屬性，請將變數部分依照以下邏輯調整後直接填入 URL 設定中
   1. 連結包含「品牌自訂變數」：
      * 請使用雙括弧來表示，例：https://example.com/?abc=((key))、((url))
      * 雙括弧中只可包含大小寫英文、數字、底線
   2. 連結包含「Omnichat 系統屬性變數」 或 「自訂屬性」
      *   可直接點選變數按鈕填入

          <figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
      * 可直接輸入並使用雙大括號來表示，例：https://example.com/?abc=\{{key\}}
      * 雙大括弧中只可包含&#x20;
        * Omnichat 支援的系統變數
        * 尚未封存的自訂屬性

***

## 發送 LINE Flex Message 方式

### 1. Open API&#x20;

* 透過 Open API / Messaging / Send Direct Message 發送訊息，發送訊息格式請參考：[https://documenter.getpostman.com/view/2s9YsMBC4o#aea7faeb-0ab4-4f19-b70f-a40d7004c040](https://documenter.getpostman.com/view/2s9YsMBC4o#aea7faeb-0ab4-4f19-b70f-a40d7004c040)
*   若 LINE Flex Message 設計的樣式為 Bubble（如下圖），可於 Open API 中放入多個為 Bubble 樣式的 LINE Flex Message，Omnichat 將自動將這些 Bubble 組成輪播訊息

    <figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption><p>Bubble 訊息樣式</p></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption><p>Open API 設定方式</p></figcaption></figure>

    <figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption><p>顧客端收到樣式</p></figcaption></figure>

### 2. Call an API 卡片

* 透過 Call an API 卡片發送訊息，發送訊息格式請參考：[https://docs.google.com/document/d/1NJXZEQPoJqThx4w2C2x8Dx6Dqjb6HjbPGqZbQquNabc/edit?tab=t.0#heading=h.66qnyil9pdv0](https://docs.google.com/document/d/1NJXZEQPoJqThx4w2C2x8Dx6Dqjb6HjbPGqZbQquNabc/edit?tab=t.0#heading=h.66qnyil9pdv0)
* 若 LINE Flex Message 設計的樣式為 Bubble，可於 API 中放入多個為 Bubble 樣式的 LINE Flex Message，Omnichat 將自動將這些 Bubble 組成輪播訊息（與 Open API 相同）

***

## 查看發送結果與成效

### Open API 發送紀錄

*   透過 Open API 發送後，可以在統計表 / Open API 發送紀錄中查看該則訊息的成效

    <figure><img src="../../.gitbook/assets/image (476).png" alt=""><figcaption><p>Open API 發送紀錄</p></figcaption></figure>



    <figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption><p>單則發送紀錄成效</p></figcaption></figure>

### 對話

*   可以在對話中找到發送的 LINE Flex Message 編號與名稱

    <figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

