---
description: 💡使用受眾管理功能的上傳受眾包至LINE 廣告平台前需要完成串接LINE 廣告帳號
---

# 串接 LINE 廣告帳號

### 串接 LINE 廣告帳號路徑：

Omnichat 系統後台**通訊渠道**＞**串接社群通訊渠道** > **LINE** > **LINE 廣告帳號**

串接時需要填寫以下資訊：

1. 群組 ID
2. API 存取金鑰
3. API 密鑰

<figure><img src="../../../.gitbook/assets/image (14) (1).png" alt=""><figcaption></figcaption></figure>

### 取得群組 ID 的方法

1. 登入 [**LINE 廣告帳號平台**](https://admanager.line.biz/home/)
2. 點選"廣告群組"
3. 紅框位置為群組 ID&#x20;

<figure><img src="../../../.gitbook/assets/image (15) (1).png" alt=""><figcaption></figcaption></figure>

### 取得API 存取金鑰與API 密鑰方法

1. 登入 [**LINE 廣告帳號平台**](https://admanager.line.biz/home/)
2. 於"設定" 點選 "群組設定"

<figure><img src="../../../.gitbook/assets/image (16) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (21) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
串接完成後若於 LINE 廣告後台重新產生密鑰，將會使串接失效，須重新串接
{% endhint %}

3. &#x20;回到 Omnichat 後台取得 Omnichat IP 後貼在"允許 API 存取的 IP 位址" 的欄位。

<figure><img src="../../../.gitbook/assets/image (18) (2).png" alt=""><figcaption></figcaption></figure>

4. &#x20;關於取得 Omnichat IP 的路徑： 通訊渠道＞串接社群通訊渠道 > LINE > LINE 廣告帳號

<figure><img src="../../../.gitbook/assets/image (19) (1).png" alt=""><figcaption></figcaption></figure>

5. 資料填寫後勾選要串接的 LINE 帳號
6. 串接完成

<figure><img src="../../../.gitbook/assets/image (20) (1).png" alt=""><figcaption></figcaption></figure>
