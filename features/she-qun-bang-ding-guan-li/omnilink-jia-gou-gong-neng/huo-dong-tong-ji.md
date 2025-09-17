---
description: 活動統計可以查看每次活動的相關成效
---

# 活動統計

<figure><img src="../../../.gitbook/assets/截圖 2024-09-20 下午3.37.37.png" alt=""><figcaption></figcaption></figure>

* 點擊動作 > 活動統計，可查看每次活動的相關成效

<figure><img src="../../../.gitbook/assets/截圖 2024-09-20 下午3.50.15.png" alt=""><figcaption></figcaption></figure>

1. 來源渠道：來源渠道名稱
2. 目標渠道：目標渠道名稱
3. 參與人數：觸發卡片且第一次點擊按鈕的次數（參與人數 = 整合成功人數 + 整合失敗人數）
4. 目標渠道 - 新聯絡人：整合成功且從未存在於團隊中的 channel 聯絡人\
   （ex. 王小明原本是品牌的 FB 聯絡人，透過 OmniLink 成為 LINE 聯絡人，此時就會被認列為新聯絡人
5. 整合成功人數：觸發卡片且點擊後整合成功人數
6. 整合失敗人數：
   * 觸發卡片且點擊後有儲存錯誤原因的人數
   * 沒有錯誤原因人數（點過去沒有整合成功）
7. 日期區間：可篩選活動期間

#### 整合成功名單

<figure><img src="../../../.gitbook/assets/截圖 2024-09-20 下午3.43.37.png" alt=""><figcaption></figcaption></figure>

1. 整合成功名單：這邊會顯示整合成功名單
2. 來源渠道 - 姓名：顯示整合成功聯絡人的來源渠道姓名
3. 來源渠道 ID：會顯示聯絡人的來源渠道 ID
4. 目標渠道 - 姓名：顯示整合成功聯絡人的目標渠道姓名
5. 目標渠道 ID：會顯示聯絡人的目標渠道 ID
6. 參與時間：客人點擊 OmniLink 的時間
7. 整合成功時間：整合成功時間
8. 匯出名單：整合成功 & 失敗的名單會一起匯出（須先選擇時間區間，且天數須小於 90 天才可匯出）

<figure><img src="../../../.gitbook/assets/截圖 2024-09-23 下午4.56.01.png" alt=""><figcaption></figcaption></figure>

#### 整合失敗名單

<figure><img src="../../../.gitbook/assets/截圖 2024-09-23 下午5.13.38.png" alt=""><figcaption></figcaption></figure>

1. 整合失敗名單：這邊會顯示失敗名單
2. 來源渠道 - 姓名：顯示失敗聯絡人的來源渠道姓名
3. 來源渠道 ID：來源渠道的 ID
4. 參與時間：參與時間
5. 失敗原因：

<table><thead><tr><th width="273">錯誤種類</th><th>錯誤訊息（中文）</th><th>後台錯誤訊息（英文）</th></tr></thead><tbody><tr><td>無法產生 deeplink</td><td>跨社群一鍵整合已停用</td><td>Cross channel connect is disabled.</td></tr><tr><td>無法產生 deeplink</td><td>無法產生整合連結</td><td>Failed to generate connect link.</td></tr><tr><td>收到「聯絡人點擊了 deep link」的通知後，要做跨社群整合時失敗</td><td>跨社群一鍵整合已停用</td><td>Cross channel connect is disabled.</td></tr><tr><td>收到「聯絡人點擊了 deep link」的通知後，要做跨社群整合時失敗</td><td>無法找到來源渠道聯絡人</td><td>Source contact not found.</td></tr><tr><td>收到「聯絡人點擊了 deep link」的通知後，要做跨社群整合時失敗</td><td>無法找到目標渠道聯絡人</td><td>Target contact not found.</td></tr><tr><td>收到「聯絡人點擊了 deep link」的通知後，要做跨社群整合時失敗</td><td>會員編號衝突</td><td>Member ID conflict.</td></tr><tr><td>收到「聯絡人點擊了 deep link」的通知後，要做跨社群整合時失敗</td><td>伺服器錯誤</td><td>Internal server error.</td></tr><tr><td>其他未預期錯誤</td><td>因顧客未送出整合訊息或未安裝目標渠道 APP 失敗</td><td>The integration might have failed because the customer didn't submit the integration message or hasn't installed the target channel app.</td></tr></tbody></table>

* 當發生以下幾種狀況時，消費者收到「此連結不存在，請洽客服詢問」 （不會顯示在失敗原因中，會直接發送訊息給客戶）

a. 找不到整合設定\
b. 整合設定已停用\
c. 找不到來源渠道\
d. 在非來源渠道觸發跨社群一鍵整合卡片\
e. 找不到目標渠道\
f. 目標渠道是 LINE 而且沒有設定綁定 LIFF ID

* 當發生以下幾種狀況時，不會顯示失敗原因

a. 整合成功\
b. 發訊息失敗\
c. 觸發旅程失敗\
d. 貼標籤失敗\
e. 各平台發生錯誤
