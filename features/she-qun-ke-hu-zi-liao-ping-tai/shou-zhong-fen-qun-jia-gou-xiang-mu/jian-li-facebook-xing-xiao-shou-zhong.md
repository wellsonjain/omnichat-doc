---
description: 行銷受眾💡支援從 Facebook 帳號中新增受眾名單至 Facebook 廣告後台
---

# 建立 Facebook 行銷受眾

### 建立 Facebook 行銷受眾

1. 至 受眾分群 > Facebook 行銷訊息受眾，點擊「建立受眾」，選擇「Facebook 行銷受眾」

<figure><img src="../../../.gitbook/assets/截圖 2026-01-25 晚上8.22.56.png" alt=""><figcaption></figcaption></figure>

2. 選擇之後要推播的 Facebook 通訊渠道與廣告帳號
3. 編輯受眾的名稱與描述，此資訊也會同步到 Meta 後台的廣告受眾
4. 以顧客的 **電話** 或 **Email**，按照範例檔案格式上傳為受眾名單（比對方式：當上傳的 電話 或 Email 有對應的 Facebook 帳號即可完成比對，帳號並不須追蹤或與 Facebook 專頁對話過）

{% hint style="info" %}
電話格式為含國碼的國際格式（e.g. ✅ 886911111111 ❌ 0911111111 ❌ +886 911111111）
{% endhint %}

<figure><img src="../../../.gitbook/assets/截圖 2026-01-25 晚上8.25.36.png" alt=""><figcaption><p>設定受眾包名稱、通訊渠道、廣告帳號與受眾描述。並下載「電話或Email」的範例檔案。</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/截圖 2026-02-04 下午5.28.44.png" alt=""><figcaption><p>上傳至 Google 試算表編輯，編輯完成後下載成 CSV 檔</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/截圖 2026-02-04 下午5.31.43 (1).png" alt=""><figcaption><p>再次回到受眾設定介面上傳 CSV 檔</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/截圖 2026-02-04 下午5.32.05.png" alt=""><figcaption><p>按下上傳後，即顯示名單上傳中畫面</p></figcaption></figure>



### 等待 Meta 完成受眾比對

1. 上傳名單後，Meta 會在約 24 小時內完成比對，比對成功的顧客就會成為一個推播對象（但基於 Meta 的隱私政策，我們無法得知是哪一位顧客比對成功）
2. **僅有當比對結果有**<mark style="color:$danger;">**100 人以上**</mark>**時，Meta 才允許使用該受眾推播**（若未達 100 人，則如下方截圖的總人數顯示「-」）

<figure><img src="../../../.gitbook/assets/截圖 2026-02-04 下午5.43.30.png" alt=""><figcaption><p>上傳狀態 - 處理中：等待 Meta 比對名單中</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/截圖 2026-02-04 下午5.44.16.png" alt=""><figcaption><p>上傳狀態 - 上傳完成：Meta 比對完成</p></figcaption></figure>



### 針對既有受眾增加名單

可針對已建議的受眾名單，繼續追加名單。點選「新增名單」，一樣依照上面建立 Facebook 行銷受眾的方式新增即可。

<figure><img src="../../../.gitbook/assets/截圖 2026-02-06 上午11.42.20.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Facebook 行銷受眾推播的限制

* 上傳名單後約 24 小時內完成比對；**比對成功的用戶即可成為可推播對象**
* 基於 Meta 隱私政策，我們無法得知哪些顧客比對成功
* **比對成功人數需達 100 人以上**，Meta 才會允許使用該受眾
* 若使用 Facebook 行銷受眾進行推播，基於 Meta 官方現行機制影響，<mark style="color:$danger;">**無法追蹤到回應率、退訂封鎖率**</mark>
{% endhint %}

## 常見問題

### 1. Facebook 行銷受眾的比對邏輯是什麼？怎樣會比對成功？

當此 Email/電話有對應的 Facebook 帳號存在，即會比對成功。該 Facebook 帳號不需要已經跟專頁對話互動過

### 2. 可以從後台建立 Facebook 行銷受眾嗎

目前 Omnichat 提供：建立行銷受眾、上傳名單、查看上傳比對狀態，無需進入 Meta Ads Manager 建立

### 3. 為什麼建立 Facebook 行銷受眾後需要等 24 小時才能開始推播？能不能更快？

受限於 Meta 的規則：

* 上傳名單後，系統需要**最多 24 小時**進行比對。目前沒有加速機制，24 小時為 Meta 官方標準

### 4. 建立的 Facebook 行銷受眾可以在其他 Meta 廣告使用嗎

不行，可以從 Meta Ads Manager 看到阻擋

<figure><img src="../../../.gitbook/assets/Screenshot 2025-12-18 at 6.22.53 AM.png" alt=""><figcaption></figcaption></figure>

### 5. 為什麼 Facebook 行銷受眾比對的人數這麼低？怎麼提高？

常見原因：

1. 名單品質低（電話格式錯誤、Email 不完整）
2. 用戶沒有使用對應的 FB 帳號

提升方式：

1. 確認電話格式為含國碼的國際格式（e.g. ✅ 886911111111 ❌ 0911111111 ❌ +886 911111111）
2. 改善 CRM 名單格式與資料完整性
3. 儘量使用 第一方資料（購買紀錄、會員資料）

### 6. 行銷受眾的比對是一次還是持續性的？

每次針對既有受眾包增加名單後就會再次比對，名單也會隨著 Meta 偵測到用戶狀態變化而更新（例如取消訂閱）



