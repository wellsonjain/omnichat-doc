---
description: >-
  Omnichat 支援製作 Facebook / Instagram 貼文留言自動回覆及貼文私訊回覆功能，讓用戶可以透過 Omnichat 製作
  Facebook / Instagram 貼文自動廣告活動
---

# Facebook / Instagram 貼文回覆

![](<../../../.gitbook/assets/截圖 2022-07-28 上午11.20.33.png>)

{% hint style="info" %}
請留意，如欲使用「Facebook 貼文回覆」功能，必須是以 Facebook 粉專管理員身份登入Facebook 粉絲專頁的狀態下才能使用，若非登入狀態則不能使用。
{% endhint %}

{% hint style="warning" %}
設定時請留意，在 Facebook / Instagram 貼文回覆活動中的關鍵字條件，英文字母與數字符號的**大、小寫，全形及半形，均會視為不同的字元。**

舉例來說：

情況一：`ABC` (半形且大寫) ，`ＡＢＣ` (全形)、`abc`（小寫），三者均為不同的關鍵字條件

情況二：關鍵字設定為 **`abc`**（半形）

客人回覆答案為：`abc` > 這個會觸發貼文/私訊回覆活動

客人回覆答案為：`Abc / ABC / aBC / ａｂｃ` > 這些不會觸發貼文 / 私訊回覆活動
{% endhint %}

## **如何設定** Facebook / Instagram 貼文回覆活動

### 步驟 **1 - 新增活動**

點選右上角的「**新活動**」按鈕

![](<../../../.gitbook/assets/截圖 2022-07-18 下午6.43.25.png>)

### 步驟 2 - 設定活動名稱及目標 Facebook / Instagram 專頁

* 輸入活動名稱
* 設定 Facebook / Instagram 專頁

<figure><img src="../../../.gitbook/assets/留言回覆標記朋友2" alt=""><figcaption></figcaption></figure>

### 步驟 3 - 選擇 Facebook / Instagram 貼文 / 手動輸入貼文編號

在「**貼文**」清單中，選擇你需要發佈「**自動回覆**」的「**貼文**」

{% hint style="info" %}
**貼文清單** 只會顯示 Facebook 粉專最近 **50** 篇「**已發佈**」的貼文

Instagram 顯示近期 **25** 篇「**已發佈**」的貼文
{% endhint %}

![](<../../../.gitbook/assets/截圖 2022-01-06 下午5.52.29.png>)

如想設定 Facebook「 **排程中貼文**」、『**廣告貼文**」或**舊貼文**你可以手動輸入貼文編號。

{% hint style="info" %}
詳細可參考「[**如何獲得 Facebook 貼文編號?**](how-to-get-facebook-post-id.md)」
{% endhint %}

![](<../../../.gitbook/assets/截圖 2022-01-06 下午5.54.04.png>)

{% content-ref url="how-to-get-facebook-post-id.md" %}
[how-to-get-facebook-post-id.md](how-to-get-facebook-post-id.md)
{% endcontent-ref %}

{% hint style="success" %}
新增全部貼文選項，可以當作所有貼文預設的自動回覆，若有單獨貼文的回覆，則以單獨貼文的自動回覆為優先
{% endhint %}

{% hint style="info" %}
如選擇全部貼文，可以支援「已發佈」、排程中以及「廣告貼文」的所有貼文。另外，活動前所發佈的所有貼文也會支援
{% endhint %}

![](<../../../.gitbook/assets/截圖 2022-01-06 下午5.55.39.png>)

### 步驟 4 - 設定貼文回覆的有效時間

設定的有效期間過後就不再派送，若沒有要設定時限則選取永久啟用

#### Facebook 貼文

![](<../../../.gitbook/assets/截圖 2022-07-18 下午6.46.53.png>)

#### Instagram 貼文

Instagram 的「 IG 直播」，只要客人在直播間留言，就會觸發私訊自動回覆訊息。

有效時間：在這段時間區間內的所有直播，都會觸發私訊自動回覆

![](<../../../.gitbook/assets/截圖 2022-07-18 下午6.47.58.png>)

### 步驟 5 - 設定貼文回覆的觸發條件

目前支援兩種觸發條件：留言訊息關鍵字、標記朋友，可以兩者同時設定。

#### 留言訊息關鍵字

![](<../../../.gitbook/assets/4 (1).png>)

1. **為任何內容**：不用設定關鍵字，在貼文下方留言任何內容（包含圖片 / FB 貼圖），即會觸發自動回覆
2. **包含部分**：若有設定多個關鍵字時，符合到其中一個關鍵字，就可以觸發自動回覆
3. **包含所有**：若有設定多個關鍵字時，需要符合所有關鍵字，才可以觸發自動回覆
4. **完全符合**：貼文下方的回覆內容需要跟後台設定的一模一樣，所以選擇此選項時，建議只設定一個關鍵字或句子即可，若設定多個關鍵字，也只會在留言「第一個」的關鍵字時才會觸發自動回覆，留言第二個之後的關鍵字不會觸發自動回覆

舉例來說：

![](../../../.gitbook/assets/包含部分.png)

選擇「**包含部分**」時，當客人留言 1、31、24 這種有包含到「1」或「2」的字詞就可以觸發



![](../../../.gitbook/assets/包含所有.png)

選擇「**包含所有**」，客人則必須要留言 12、21 這樣有包含到「1」和「2」的字詞，才可以觸發



![](<../../../.gitbook/assets/完全符合 new.png>)

選擇「**完全符合**」，客人只有在留言「Omnichat」時（由於Omnichat 是第一個關鍵字），才可以觸發自動回覆，留言「ABC」、「Hi」 時不會觸發自動回覆。

#### 標記朋友

<figure><img src="../../../.gitbook/assets/留言回覆標記朋友1" alt=""><figcaption></figcaption></figure>

1. 不需標記：若不限制需要標記朋友，請選擇此項
2. 大於或等於：設定數量後，系統會偵測客人符合標記朋友的數量後，自動觸發回覆內容

{% hint style="info" %}
目前 Instagram 平台<mark style="color:red;">**不支援**</mark>偵測標記朋友，因此無法使用此條件。
{% endhint %}

### 步驟 6 - 設定貼文留言回覆及私訊回覆內容

設定**最少一組**的「貼文留言回覆」或「私訊回覆」。

「**私訊回覆**」內容支援2種類型：

1. 「**文字**」：以純文字私訊回覆，可以添加姓名參數自動顯示聯絡人名稱。
2. 「**機器人卡片**」：以機器人卡片模組回覆（注意：因為 Facebook 的限制，只可以回覆**包含 1 張卡片**的模組，建議使用有按鈕的卡片，可提高用戶跟粉專的互動率）

{% hint style="danger" %}
設定多個回覆訊息，系統會隨機選擇其中一個訊息回覆給使用者。如此可以避免每次自動回覆的訊息都相同，降低 Facebook/IG 帳號被 Meta 端封鎖的機會。
{% endhint %}

{% hint style="info" %}
選擇以「**文字**」回覆時，可以點選輸入框右下的藍色框框選取【聯絡人名稱】，系統會在內容中帶入 \{{system:cutomer\_name\}} 的姓名參數，會自動抓取聯絡人社群名稱。
{% endhint %}

<figure><img src="../../../.gitbook/assets/截圖 2022-12-07 下午12.12.54.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/FB圖文回覆功能-客戶呈現.png" alt=""><figcaption><p>以上畫面為客人收到貼文回覆與私訊的畫面</p></figcaption></figure>

### 步驟 7 - 添加多組貼文留言回覆及私訊回覆內容

你亦可以設定**多組**貼文留言回覆及私訊回覆

![](../../../.gitbook/assets/fb-cm-reply-bot-2.png)

### 支援消費者在限時動態標註 Instagram 官方帳號可收到私訊回覆

{% hint style="danger" %}
消費者 Instagram 帳號需為「公開」，否則若在「private」狀態無法觸發私訊給消費者內容。
{% endhint %}

#### 步驟一：先選擇貼文內容為「IG 限動標註」

![](<../../../.gitbook/assets/截圖 2022-07-28 上午11.30.28.png>)

#### 步驟二：可依照行銷活動設計期限：永久啟用或是時間排程

![](<../../../.gitbook/assets/截圖 2022-07-28 上午11.30.46.png>)

#### 步驟三：到「回覆設定」中進行私訊內容設定，可選擇文字或機器人模組

{% hint style="info" %}
選擇以「**文字**」回覆時，可以點選輸入框右下的藍色框框選取【聯絡人名稱】，系統會在內容中帶入 \{{system:cutomer\_name\}} 的姓名參數，會自動抓取聯絡人社群名稱。
{% endhint %}

<figure><img src="../../../.gitbook/assets/截圖 2022-12-07 下午1.33.31.png" alt=""><figcaption></figcaption></figure>

#### 當客人標註帳號時即會自動發訊息

![](<../../../.gitbook/assets/截圖 2022-07-28 上午11.39.05.png>)

### 支援消費者在 Reels 貼文留言時觸發「自動回覆」&「私訊回覆」

<figure><img src="../../../.gitbook/assets/截圖 2023-06-15 上午10.47.48 (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/截圖 2023-06-15 上午10.50.48.png" alt=""><figcaption></figcaption></figure>

1. 設定活動名稱
2. 設定渠道
3. 選擇FB/IG帳號
4. 選擇已經建立好的 Reels 貼文
5. 設定留言內容
6. 設定貼文留言回覆
7. 設定私訊留言回覆

<div><figure><img src="../../../.gitbook/assets/IMG_4155.jpg" alt=""><figcaption></figcaption></figure> <figure><img src="../../../.gitbook/assets/IMG_4156 (1).PNG" alt=""><figcaption></figcaption></figure></div>

## 列表功能

![](<../../../.gitbook/assets/截圖 2022-07-18 下午6.56.46.png>)

1. 草稿：草稿狀態下的貼文可以進去編輯修改貼文，一但發布之後只能暫停
2. 已暫停：只要啟用狀態按下暫停就會顯示，即便符合自動回覆條件也不會觸發
3. 列表頁帳號欄位後方會依據設定的貼文選項顯示：**單則貼文、全部貼文、IG直播**
4. 編輯：如需要進行修改，點擊編輯進去修改該設定
5. 啟動：可對「草稿」及「已暫停」的貼文活動進行設定
6. 暫停：按下該按鈕就會讓貼文活動呈現「已暫停」
