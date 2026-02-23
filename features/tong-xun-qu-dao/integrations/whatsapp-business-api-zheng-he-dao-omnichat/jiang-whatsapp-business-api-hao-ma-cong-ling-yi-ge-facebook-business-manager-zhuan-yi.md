---
description: 若您無法依照既有 WhatsAppB Business API 號碼串接方式進行執行，則可參考本篇的做法
---

# 將 WhatsApp Business API 號碼從另一個 Facebook Business Manager 轉移



{% hint style="info" %}
**使用背景說明**

1. 目前無法找到具有「完整存取權限（Full Access）」角色的人員登入企業管理平台（簡稱 FBM）。\
   請留意，**操作者必須使用擁有管理員角色 FB 帳號登入**，才能授權使用 MM Lite API。
2. WhatsApp 帳號的付款方式尚未設定為 Omnichat。
3. 共存模式（Coexistence）的 WABA 需要轉移至新的 FBM。
{% endhint %}

## 請依照您的需求查看步驟

[情況一、使用者擁有原本企業管理平台（ Facebook Business Manager ）的管理員權限](jiang-whatsapp-business-api-hao-ma-cong-ling-yi-ge-facebook-business-manager-zhuan-yi.md#fbm-admin-access)

[情況二、使用者沒有企業管理平台（Facebook Business Manager）的管理員權限](jiang-whatsapp-business-api-hao-ma-cong-ling-yi-ge-facebook-business-manager-zhuan-yi.md#qing-jing-er-shi-yong-zhe-mei-you-fbm-guan-li-yuan-quan-xian)

## 情況一：使用者擁有原 FBM 的管理員權限。 <a href="#fbm-admin-access" id="fbm-admin-access"></a>

步驟一：前往 FBM 中的 WhatsApp 帳號頁面，然後刪除該電話號碼。

<figure><img src="../../../../.gitbook/assets/image (544).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (545).png" alt=""><figcaption></figcaption></figure>

步驟二：透過嵌入式註冊流程（embedded signup flow），將該電話號碼連接至新的 WABA（位於另一個 FBM 底下）。

<figure><img src="../../../../.gitbook/assets/image (546).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (547).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
您需要選擇另一個 WABA（或建立一個新的 WABA）來連接該電話號碼。
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (548).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (549).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (550).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (551).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (552).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (553).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (554).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (555).png" alt=""><figcaption></figcaption></figure>

## 情況二：使用者<mark style="color:$danger;">**沒有**</mark> FBM 管理員權限。

#### （此方式同樣適用於擁有 FBM 管理員權限的情況） <a href="#fbm-no-admin-access" id="fbm-no-admin-access"></a>

{% hint style="danger" %}
請留意，由於 Meta API 行為的變更，以下嘗試可能無法成功的機率發生。
{% endhint %}

步驟一：關閉雙重驗證。

<figure><img src="../../../../.gitbook/assets/image (556).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (557).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (558).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (559).png" alt=""><figcaption></figcaption></figure>

您將會在個人的 Facebook 電子信箱中收到一封標題為「Two-Step Verification Reset」的郵件。請開啟該郵件，並點擊內文連結以繼續完成驗證流程。

<figure><img src="../../../../.gitbook/assets/image (560).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (561).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (562).png" alt=""><figcaption></figcaption></figure>

步驟二：在新的 FBM 中，選擇目標 FBM 與 WABA 帳號，接著選擇現有的電話號碼，並將該電話號碼新增進去。

<figure><img src="../../../../.gitbook/assets/image (563).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (564).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
您需要選擇另一個 WABA（或建立一個新的 WABA）來連接該電話號碼。
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (565).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (566).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (567).png" alt=""><figcaption></figcaption></figure>

{% columns %}
{% column %}
情況一：\
如果畫面上出現黃底訊息，表示可以進行遷移。



<figure><img src="../../../../.gitbook/assets/image (570).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
情況二：\
如果畫面以紅色標示，表示無法進行轉移。<mark style="color:$danger;">您需要先在 Meta 後台移除該電話號碼（如</mark>[<mark style="color:blue;">**情境一**</mark>](jiang-whatsapp-business-api-hao-ma-cong-ling-yi-ge-facebook-business-manager-zhuan-yi.md#qing-jing-yi-shi-yong-zhe-reng-yong-you-yuan-fbm-de-guan-li-yuan-quan-xian)<mark style="color:$danger;">步驟）</mark>。<mark style="color:$danger;">若您沒有權限移除，則無法繼續操作。請注意，您可能需要自行尋找具有完整操作權限的人員。</mark>

<figure><img src="../../../../.gitbook/assets/image (571).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

如果可以進行遷移，則可繼續操作。

<figure><img src="../../../../.gitbook/assets/image (568).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (552).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (553).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (554).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (555).png" alt=""><figcaption></figcaption></figure>
