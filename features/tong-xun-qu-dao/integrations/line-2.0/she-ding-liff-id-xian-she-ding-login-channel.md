---
description: >-
  不管是社群身份綁定要免除六位數驗證碼步驟 ，還是遊戲模組使用在 LINE 官方帳號上，皆需要先有 LIFF ID，設定 LIFF ID 前需要先設定好
  Login Channel
---

# 設定 LIFF ID – 先設定 Login Channel

## 設定 Login Channel 前，先確認是否已經有 LINE 官方帳號相對應的 Messaging API Channel 以及 Provider

您可以從 LINE Official Account Manager（Line OA 後台）->「設定」-> 「Messaging API」-> 點擊 「LINE Developers」 進入

<figure><img src="../../../../.gitbook/assets/截圖 2022-01-03 上午11.34.26.png" alt=""><figcaption></figcaption></figure>

#### 如您進到 LINE OA 原生後台顯示如下圖，表示您沒有開啟過 Messaging API Channel，請略過以下步驟，並至 [LINE 官方帳號整合到 Omnichat 的步驟一](line2.0.md#bu-zhou-yi)接續完成。

提醒您：一旦開啟後，該 LINE 登入帳號也視為 Messaging API Channel 管理員帳號且無法變更。若您非該官方帳號擁有者或是非主管，請讓主管或是擁有者進行開啟 Messaging API 後並分享權限給您。

{% hint style="info" %}
LINE 官方帳號內管理員權限不代表擁有 Messaging API Channel 權限，兩者為分開獨立，請特別注意！
{% endhint %}

<figure><img src="../../../../.gitbook/assets/LINE OA 尚未開啟 Messaging API Channel .png" alt=""><figcaption></figcaption></figure>

### 如貴司 LINE 官方帳號已開啟 Messaging API Channel，點擊後請點右上角人像處，並點擊 LINE Console

<figure><img src="../../../../.gitbook/assets/LINE Console.png" alt=""><figcaption></figcaption></figure>

#### 若您已經取得 Messaging API Channel 和相對應 Provider，則您畫面會如下圖：

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午3.20.55.png" alt=""><figcaption></figcaption></figure>

1. 可新增 Channel 的按鈕
2. Messaging API Channel（裡面的 Bot basic ID 等於 LINE@ ID）
3. Provider 名稱及它在「Admin」名稱下方

#### 情況一：如您登入後需要您重新創建一個 Provider（如下圖顯示）表示您沒有該 Messaging API Channel 及對應 Provider 帳號。

#### 請洽當時創建同仁授權。如果無法聯繫當時開啟權限同仁，請洽 LINE 官方客服請求拿回 Messaging API Channel 和對應 Provider 權限。

<figure><img src="../../../../.gitbook/assets/LINE Console-1.png" alt=""><figcaption></figcaption></figure>

#### 情況二：若您在畫面如下，左側選單顯示 Channel 名稱在「No role」底下，請先點擊進到 Messaging API Channel 內確認是否與您所要連接的 LINE 官方帳號相同

<div><figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午1.47.39.png" alt=""><figcaption><p>點進去該 Channel 內選擇「Messaging API」分頁</p></figcaption></figure> <figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午1.53.33.png" alt=""><figcaption><p>確認 LINE ID 是否相符</p></figcaption></figure></div>

如相符，則您目前僅拿到 Messaging API Channel 權限，您需要取得 Provider 權限才能進行下一步！

{% hint style="info" %}
每一個 LINE 官方帳號都僅連接一個 Messaging API Channel，您無法自行創建一個\
因此，**請務必找到相對應的 Messaging API Channel 及 Provider**\
後續創建的 Login channel 及 LIFF ID 才會是正確的
{% endhint %}

### 如何取得 Provider ＆ Messaging API Channel 權限

#### 請有權限的同仁先確認畫面

只要畫面上 Admin 旁有 Provider 名稱，以及 Provider 內有 Messaging API Channel，請先點擊「Role」

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午4.17.52.png" alt=""><figcaption></figcaption></figure>

#### 接下來點擊按鈕「Invite by e-mail」

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午4.26.04.png" alt=""><figcaption></figcaption></figure>

輸入 E-mail 和選擇 Role 為「Admin」，並點擊按鈕「Send invitations」

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午4.41.34.png" alt=""><figcaption></figcaption></figure>

然後點擊 Messaging API Channel 進到裡面後，點擊「Roles」

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午5.29.51.png" alt=""><figcaption></figcaption></figure>

點擊裡面的按鈕「Invite by email」，填入要授權的 E-mail 和選擇 Role 為「Admin」，並點擊按鈕「Send invitations」

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午5.39.12.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午4.41.34.png" alt=""><figcaption></figcaption></figure>

可至 E-mail 信箱內收信件，點擊超連結「Accept the invitation」

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午5.42.56.png" alt=""><figcaption></figcaption></figure>

## 已有 Login Channel

如果您按照前方步驟進到畫面後，發現有看到 login channel。\
但看到 Channel 反灰左上方顯示 no role，也無法點擊進入，表示您沒有權限。請其他有權限的同仁提供您該 Channel 的 Admin 權限。（請參考上方：如何取得 Messaging API Channel 權限步驟）

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午5.45.17.png" alt=""><figcaption></figcaption></figure>

取得 Login Channel 權限後，請點擊進到 Login Channel 的 Basic Setting 分頁內確認 **Linked OA** 是否有連結。如有的話請按照下方步驟看您是要設定 LINE 遊戲模組 LIFF ID，還是要設定 LINE 社群身份綁定 LIFF ID

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午6.15.49.png" alt=""><figcaption></figcaption></figure>

{% content-ref url="you-xi-mo-zu-zhuan-yong-line-liff-id-she-ding.md" %}
[you-xi-mo-zu-zhuan-yong-line-liff-id-she-ding.md](you-xi-mo-zu-zhuan-yong-line-liff-id-she-ding.md)
{% endcontent-ref %}

{% content-ref url="she-qun-shen-fen-bang-ding-liff-she-ding.md" %}
[she-qun-shen-fen-bang-ding-liff-she-ding.md](she-qun-shen-fen-bang-ding-liff-she-ding.md)
{% endcontent-ref %}

## 尚未建立 Login Channel  <a href="#nothaveloginchannel" id="nothaveloginchannel"></a>

在取得 Provider 和 Messaging API Channel 權限後，該 Provider 內沒有 login channel 時，則可以開始建立 login channel 來取得後續 LIFF ID 設定

### 步驟一

* 點選 Create a new channel
* 選擇 LINE Login

<div><figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午5.58.11.png" alt=""><figcaption></figcaption></figure> <figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午5.58.40.png" alt=""><figcaption></figcaption></figure></div>

### 步驟二：填寫 Login Channel 內的資訊

<figure><img src="../../../../.gitbook/assets/截圖 2021-12-09 下午6.30.03.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/截圖 2021-12-09 下午6.38.22 (1).png" alt=""><figcaption></figcaption></figure>

1. Channel Type：LINE Login（固定）
2. Provider：為您們原先 Provider 名稱
3. Region 選擇 **Taiwan**
4. Channel icon 用 貴司官方帳號的 icon
5. Channel name 為 貴司的 LINE 官方帳號名稱
6. Channel Description – LINE 好友要玩遊戲前會有允許權限的流程，會顯示這個描述，所以請不要複製上方文字，請描述該認證流程。如您不知道該填寫什麼內容，可填寫品牌名稱
7. App types 兩個都勾選
8. 勾選『 I have read and agree to the LINE Developers Agreement』
9. 點選 create

### 步驟三：將 Login Channel 調整為 Published

點擊 Create 後會進到創建好的 login channel，在上方「Developing」點擊後會彈出視窗，點擊「Publish」將 Channel 狀態調為 Published

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午6.30.20.png" alt=""><figcaption></figcaption></figure>

### 步驟四：調整 Login Channel 連結 LINE 官方帳號

在 Basic Setting 分頁內，往下滑至 **Linked OA** 處，選擇要連結的 LINE 官方帳號後，點擊按鈕「Update」

<figure><img src="../../../../.gitbook/assets/截圖 2022-10-24 下午6.22.56.png" alt=""><figcaption></figcaption></figure>

#### 設定完畢後，請依照您是要設定 LINE 遊戲模組 LIFF ID，還是要設定 LINE 社群身份綁定 LIFF ID

{% content-ref url="you-xi-mo-zu-zhuan-yong-line-liff-id-she-ding.md" %}
[you-xi-mo-zu-zhuan-yong-line-liff-id-she-ding.md](you-xi-mo-zu-zhuan-yong-line-liff-id-she-ding.md)
{% endcontent-ref %}

{% content-ref url="she-qun-shen-fen-bang-ding-liff-she-ding.md" %}
[she-qun-shen-fen-bang-ding-liff-she-ding.md](she-qun-shen-fen-bang-ding-liff-she-ding.md)
{% endcontent-ref %}
