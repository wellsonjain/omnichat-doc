---
description: 您可以新增以下代碼在網站按鈕觸發上，即可同時開啟聊天插件
---

# 按鈕事件

```
let omnichatButton = document.getElementById('easychat-floating-button');
let event = new Event('click');
omnichatButton.dispatchEvent(event);
```
