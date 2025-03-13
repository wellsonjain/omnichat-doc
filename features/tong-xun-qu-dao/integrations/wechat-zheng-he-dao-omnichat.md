# WeChat | 整合到 Omnichat

## 步驟一

首先要登入到微信的後台（https://mp.weixin.qq.com/）

{% embed url="https://mp.weixin.qq.com/" %}

<figure><img src="../../../.gitbook/assets/Screenshot 2022-11-08 at 6.23.27 PM.png" alt=""><figcaption></figcaption></figure>

## 步驟二

#### 在手機中打開WeChat 按右上角 `+` 的符號 選「`掃描」` 或 「`Scan」`

![](<../../../.gitbook/assets/Screenshot 2022-11-08 at 6.02.12 PM.png>)

## 步驟三

#### 1.  用手機掃描電腦瀏覽器中的 QR Code 後，在手機中選擇需要登錄的帳號

![](../../../.gitbook/assets/photo_6293849598615204816_y.jpeg)

#### 2.  選擇需要登錄的帳號後 電腦瀏覽器會自動登入到WeChat的後台&#x20;

#### 3.  然後在左列選單選擇進入「**設置與開發」** 裡的 「**基本配置」**

<figure><img src="../../../.gitbook/assets/Screenshot 2022-11-09 at 2.02.54 PM.png" alt=""><figcaption></figcaption></figure>

#### 4.  進入**基本配置頁面**後，複製 _**開發者ID（AppID）**_ 和 _**`開發者密碼 (AppSecret)`**_ 給 Omnichat 的工作人員

<figure><img src="../../../.gitbook/assets/Screenshot 2022-11-09 at 2.09.04 PM.png" alt=""><figcaption></figcaption></figure>

## 步驟四

#### 1.  您畫面中的服務器配置可能尚未啟用，請先調整為「啟用 」，然後按「修改配置」

<figure><img src="../../../.gitbook/assets/Screenshot 2022-11-09 at 2.09.04 PM copy.png" alt=""><figcaption></figcaption></figure>

#### 2. 在服務器配置中，您需要填入 `URL` `Token` `EncodingAESKey`這三項資訊 並選擇`明文模式`&#x20;

這三項資訊請向 Omnichat 工作人員索取

<figure><img src="../../../.gitbook/assets/Screenshot 2022-11-09 at 2.19.20 PM.png" alt=""><figcaption></figcaption></figure>

## 步驟五 按`提交`後即完成整合



