---
description: 本頁說明如何在Omnichat後台做可用餘額儲值與付款。
---

# 付款與儲值

<figure><img src="../../../.gitbook/assets/截圖 2025-01-07 下午5.23.10.png" alt=""><figcaption></figcaption></figure>

### 1. 可用餘額

可用餘額（每小時試算） = 交易紀錄餘額 - 未出帳用量（每小時試算）- 累計未付月結帳單

#### 1.1 展開更多資訊

<figure><img src="../../../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

* 交易紀錄餘額：等於交易紀錄頁最新的餘額（包含月結帳單和每次成功儲值紀錄）
* 未出帳用量（每小時試算）：從每月 1 號的凌晨 00:00 分開始的試算用量（每小時整點更新）
* 累積未付月結帳單：帳單裡所有未付月結帳單金額總和
* 本月已沖銷月結帳單：本月已沖銷的月結帳單金額總和
* 本月儲值加總：本月的儲值金額總和

{% hint style="danger" %}
- 當帳戶可用餘額低於「最低寬限金額」，系統會自動暫停一切須儲值的功能使用，如 WhatsApp 訊息發送、LINE 通知型訊息發送、簡訊發送及 Live Video。
-   每個團隊可用餘額的 「過低警示金額」 ，將依據每個幣別的預設值來做判斷，不同幣別的預設如下：

    * HKD：3500
    * MYR：50
    * USD：100
    * SGD：100
    * TWD：5000

    _<mark style="color:blue;">**＊若有需要調整餘額最低預設值，請向您的客戶顧問/經理洽詢**</mark>_
{% endhint %}

### 2. 自動儲值功能的 Stripe 信用卡付款方式設定

點選設定，進入 Stripe 頁面進行信用卡設定。設定完成後，在 Omnichat 帳戶總覽後台會顯示已設定好的信用卡資料，系統將會自動使用預設信用卡來進行儲值付款。

* Omnichat 的自動儲值功能目前只支援 Stripe 信用卡方式付款（<mark style="color:red;">**請留意備註一：Stripe 信用卡付款產生的費用**</mark>）。Stripe 信用卡設定方式如下：

1. 點選設定會進入 Stripe 頁面設定，設定完成後在 Omnichat 帳戶總覽後台會顯示已設定完成的信用卡資訊
2. 系統會自動抓取預設信用卡來進行儲值付款

<figure><img src="../../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

### 3. 自動儲值

1. 需先設定 Stripe 信用卡資料，才能開啟自動儲值功能
2. 打開自動儲值金額，並設定「當可用餘額低於」&「自動儲值金額」兩個欄位的金額

{% hint style="danger" %}
1) 系統每小時會判斷可用餘額是否低於設定值，當低於設定值時會按照自動儲值金額進行自動儲值
2) 系統每完成一次自動儲值都會產生一筆帳單紀錄，同時也會通過電郵寄出儲值成功通知信
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
備註一、Stripe 信用卡付款產生的費用：\


香港地區

a. 線上支付 5 %手續費&#x20;

b. 使用非香港地區發出的信用卡會被視為海外交易，信用卡公司會收取海外交易手續費（具體收費請向信用卡公司查詢）\


台灣地區

a. 線上支付 5 %手續費&#x20;

b. 台灣地區會另外收取 5 %稅金&#x20;

c. 使用非香港地區發出的信用卡會被視為海外交易，信用卡公司會收取海外交易手續費（具體收費請向信用卡公司查詢）\


其他地區

a. 線上支付 5 %手續費&#x20;

b. 使用非香港地區發出的信用卡會被視為海外交易，信用卡公司會收取海外交易手續費（具體收費請向信用卡公司查詢）
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

香港地區

<figure><img src="../../../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>

### 4. 單次儲值(線上 / 線下）

* 線上單次儲值

<figure><img src="../../../.gitbook/assets/截圖 2025-01-07 下午5.39.30.png" alt=""><figcaption></figcaption></figure>

1. 點擊儲值，並選擇儲值方式

<figure><img src="../../../.gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

2. 點擊 「信用卡」 ，並輸入儲值金額，完成後按「付款」

<figure><img src="../../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

3. 輸入信用卡資料以完成付款。付款完成後，儲值金額會自動添加到後台餘額。系統也會通過電郵寄出儲值成功通知信

<figure><img src="../../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

* 線下單次儲值

1. 點擊 「匯款」 ，輸入本次儲值標題紀錄與儲值金額

<figure><img src="../../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

2. 點擊送出後，可以下載帳單
3. 付款完成後請上傳匯款證明，待 Omnichat 財務確認及審批匯款後，所儲值之金額將會自動添加到後台餘額。（請留意:確認及審批匯款需要至少一個工作天）

<figure><img src="../../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

### 5. 帳單紀錄

{% hint style="warning" %}
所有已付款及未付款的儲值和月結帳單均會顯示在帳單紀錄裡。客戶可以根據帳單的建立時間、類型、狀態進行篩選，並匯出結果（.csv 檔）
{% endhint %}

<figure><img src="../../../.gitbook/assets/截圖 2024-10-24 下午5.34.57.png" alt=""><figcaption></figcaption></figure>

1. 標題：會根據品牌有使用的功能項目，呈現不同項目的帳單，例如：LINE 通知型訊息帳單、WhatsApp 訊息帳單、簡訊帳單、Live Video 帳單。另外，若有進行儲值，也會出現儲值交易紀錄
2. 帳單號碼 / 建立時間：會呈現每筆帳單 or 交易紀錄的號碼與建立時間
3. 帳單金額：會出現「月結帳單金額」&「儲值交易金額」
4. 付款確認時間：會出現款項確認的時間
5. 類型：「月結」、「儲值（匯款）」、「儲值（信用卡）」\
   。月結帳單：每月初會自動產出「月結」帳單，概念與電話帳單相同，會呈現不同項目的帳單，例如：LINE 通知型訊息帳單、WhatsApp 訊息帳單、簡訊帳單、Live Video 帳單\
   。儲值（匯款）：選擇透過「儲值（匯款）」加值訊息費用\
   。儲值（信用卡）：選擇透過「儲值（信用卡）」加值訊息費用
6. 狀態：「已付款」、「待審核」、「待付款」、「已取消」、、「失敗」\
   。「已付款」：每月產出月結帳單後，若品牌有預先支付訊息費用，系統會優先以預付訊息費去支付。完成支付後，「帳單狀態」會是「已付款」\
   。「待審核」：若選擇「儲值匯款」方式支付帳單，在 Omnichat 財務人員完成對帳前，帳單狀態會是「待審核」\
   。「待付款」：每月產出月結帳單後，若預付訊息費餘額不足以支付費用，狀態會是「待付款」，可點擊動作進行付款\
   。「已取消」：該筆儲值交易已取消
7. 動作：「查看匯款證明」、「下載帳單」、「儲值」\
   。查看匯款證明：若已完成匯款，可在這邊查看匯款證明\
   。下載帳單：可下載帳單\
   。儲值：若帳單狀態為「待付款」，可點擊動作進行儲值

{% hint style="warning" %}
**待付款的儲值 / 月結帳單**：可以下載帳單、上傳匯款證明、取消儲值申請

**已付款的儲值 / 月結帳單**：可以下載帳單
{% endhint %}

8. 匯出：可匯出帳單紀錄（不同地區會有不同版本，台灣地區會有發票號碼 & 備註）

<figure><img src="../../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

### 6. 交易紀錄

所有已完成交易的儲值帳單以及月結帳單會依建立帳單時間順序（從新至舊）顯示在交易紀錄的頁面。客戶可以依時間進行篩選。

<figure><img src="../../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>
