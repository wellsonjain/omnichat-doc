# 沿用舊有電話號碼申請 WhatsApp Business API (官方商業帳號)及轉移聊天紀錄教學

您可以使用舊有電話號碼申請 WhatsApp Business API。

{% hint style="warning" %}
1. 備份在 Google Drive 或是 iCloud 無法讀取過往對話紀錄，請務必準備另一個沒有下載過 WhatsApp 的裝置和門號
2. 目前僅提供可以保存聊天記錄在原有手機上查詢，官方無法支援 WhatsApp Business 帳號用戶直接將對話記錄遷移到已成為 WhatsApp Business API 號碼的帳號
{% endhint %}

## 如果您希望保留 WhatsApp/ WhatsApp Business 帳號上的聊天紀錄，請參考以下做法:

PS. 為了理解方便，原有 WhatsApp Business 帳號號碼為 **886916000123**，對應手機為「舊手機」；\
新電話門號為 **886916000456**，對應手機為「新手機」

#### 步驟一：先準備一個新電話號碼（ 886916000456）及一部新手機裝置

#### 步驟二：在原有手機上打開 WhatsApp/ WhatsApp Business 帳戶，前往 設定 -> 對話備份 -> 立即備份

![](<../../../../.gitbook/assets/Screenshot 2022-05-31 at 3.24.09 PM.png>)

#### 步驟三：取出舊 SIM card（門號 886916000123）然後插入新手機。

#### 步驟四：請在新手機下載 WhatsApp，然後註冊原本 WhatsApp Business 帳號的手機號碼（門號 886916000123）。

#### 步驟五：在新手機上的 WhatsApp，前往設定 -> 帳戶 -> 刪除我的帳戶。刪除您的帳戶不會影響原有聊天紀錄，因為相關紀錄儲存在舊手機內。

#### 刪除帳戶後（表示已經在刪除 WhatsApp Business 帳號）， 你有可能暫時無法接收新訊息(約數個小時)，直至 WhatsApp Business API 成功串接。

![](<../../../../.gitbook/assets/Screenshot 2022-05-31 at 3.32.58 PM.png>)

#### 步驟六：在舊手機上，插入新 SIM card（門號：**886916000456**），打開 WhatsApp 並重新連接新號碼。 現在，聊天紀錄會在舊手機上顯示，但並不會轉移 至 WhatsApp Business API。

### 完成以上步驟，即可返回 Omnichat 進行 WhatsApp Business API 串接。
