---
description: 如何在 Cyberbiz 網店上安裝 Omnichat？
---

# Cyberbiz | 安裝 Omnichat

使用 Cyberbiz 開店平台商，您有兩種方式可以安裝對話插件，請擇一操作即可

1. [在 Cyberbiz 後台來安裝對話插件](https://docs.omnichat.ai/features/tong-xun-qu-dao/wang-zhan-dui-hua-cha-jian/install/cyberbiz-an-zhuang-omnichat#shi-yong-cyberbiz-hou-tai-wei-zhi-lai-an-zhuang-cha-jian)
2. [使用 Google Tag Manager 來安裝](https://docs.omnichat.ai/features/tong-xun-qu-dao/wang-zhan-dui-hua-cha-jian/install/cyberbiz-an-zhuang-omnichat#shi-yong-google-tag-manager-lai-jin-hang-an-zhuang)

## 使用 Cyberbiz 後台位置來安裝插件

### 步驟 1

[登入](https://app.easychat.co/) 到 Omnichat 管理員頁面

### 步驟 2

前往  通訊渠道  >  網站對話插件  >  [安裝對話插件](https://app.easychat.co/install.html)  頁面

1. 輸入安裝 Omnichat 的網站地址
2. 複製 Omnichat 安裝代碼
3. 設定你的開店平台，選擇 Cyberbiz 並按下儲存

![放上 Cyberbiz 網址](<../../../../.gitbook/assets/截圖 2022-02-15 下午6.39.32.png>)

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午6.39.38.png>)

### 步驟 3

登錄您的 Cyberbiz 商店管理：[https://sycafe.cyberbiz.co/user/sign\_in](https://sycafe.cyberbiz.co/user/sign_in)

### 步驟 4

1. 點選左側選單網站外觀中的『套版主題管理』
2. 點擊選擇操作後點選『CSS/HTML編輯器』

<figure><img src="../../../../.gitbook/assets/cyberbiz對話插件設定步驟-CSSHTML編輯器位置 (1).png" alt=""><figcaption></figcaption></figure>

### 步驟 5

請勾選「我已閱讀並同意上述事項」，並點選「我同意」

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午6.33.12.png>)

### 步驟 6

1. 點選「整體配置」的『theme\_liquid』
2. 將剛剛在 Omnichat 複製好的插件代碼貼在 \<body> 之後（忘記剛剛插件代碼在哪請點擊[這裡](cyberbiz-an-zhuang-omnichat.md#bu-zhou-2)）

![點擊「theme\_liquid」](<../../../../.gitbook/assets/截圖 2022-02-15 下午6.37.22.png>) ![將插件代碼放在 \<body> 之後，整段貼上](<../../../../.gitbook/assets/截圖 2022-02-15 下午6.40.21.png>)

3\. 點擊『儲存』

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午7.10.53.png>)

### 步驟 7

看到插件在網站上出現！

![左下角藍色插件已上線](<../../../../.gitbook/assets/截圖 2022-02-15 下午6.42.56 (1).png>)

## 使用 Google Tag Manager 來進行安裝

### 步驟 1

[登入](https://app.easychat.co/) 到 Omnichat 管理員頁面

### 步驟 2

前往  通訊渠道  >  網站對話插件  >  [安裝對話插件](https://app.easychat.co/install.html)  頁面

1. 輸入安裝 Omnichat 的網站地址
2. 複製 Omnichat 安裝代碼
3. 設定你的開店平台，選擇 Cyberbiz 並按下儲存

![放上 Cyberbiz 網址](<../../../../.gitbook/assets/截圖 2022-02-15 下午6.39.32.png>)

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午6.39.38.png>)

### 步驟 3

登入您的 Google Tag Manager 帳戶 [https://tagmanager.google.com](https://tagmanager.google.com/)

### 步驟 4&#x20;

如您已經創建給官網，可直接找到當時的 GTM 代碼往步驟 5 操作。

新增帳戶並設置帳戶設定及容器設定，並在「目標廣告平台」選擇「網路」，並按下「建立」。

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午7.19.22.png>)

### 步驟 5

勾選底下的「我同意」以及點擊上方的「是」

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午7.29.08.png>)

### 步驟 6

按下新增代碼，輸入標籤名稱（Tag name），然後按右上角的編輯鉛筆（Edit Pencil）

![新增代碼](<../../../../.gitbook/assets/截圖 2022-02-15 下午7.31.31.png>)

![輸入標籤名稱，以及點擊鉛筆](<../../../../.gitbook/assets/截圖 2022-02-15 下午7.33.19.png>)

### 步驟 7

選擇自訂代碼 Custom HTML

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午7.35.58.png>)

### 步驟 8

把 Omnichat Javascript 代碼 貼到 HTML Textbox。\
按下觸發條件右邊的＋，來新增條件，選擇「All Pages」

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午7.39.01.png>)

### 步驟 9

按下「提交」

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午7.42.12.png>)

### 步驟 10

如果您是之前就已經有 GTM 而修改後提交新版本，按下提交後，並添寫以下欄位後按『發布』

1. 版本名稱 Version Name：Version 1
2. 版本說明 Version Description：Add Omnichat installation code
3. 按下「發布」

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午7.45.35.png>)

### **完成！**

![](<../../../../.gitbook/assets/截圖 2022-02-15 下午6.42.56.png>)
