---
description: Conversion Analysis
---

# 轉換率分析

轉換率分析有分成「購物行為」與「來源 / 媒介」兩個區塊。當安裝 Omnichat Pixel 之後，可以查看各個來源的轉換成效。

## 日期區間

![](<../../../.gitbook/assets/image (220).png>)

* 一進到網頁的預設日期，是從今天開始算到過去 7 天（一週）
* &#x20;可以點選日期，去選擇想看到的日期區間，再按搜尋
* 搜尋新日期之後，「購物行為」與「來源 / 媒介」的數據都會同時被更新

## 工作階段 Session

* 這裡的工作階段 Session 跟 Google Analytics 的工作階段定義是相似的
* 當一個訪客進到網站的第一個頁面（Landing Page）時，便會開啟一個工作階段（Session），而一個工作階段裡面會包含不同的行為（Behavior）
* 我們這裡目前可以看到的行為抱括：
  * 把商品加入購物車的動作
  * 開始結帳的動作
  * 完成訂單交易的動作
* 通常在同一個工作階段開啟之後，只要訪客在網站上有持續的互動，所有的行為都會被算在該工作階段裡面，但有兩個情況會再開啟另一個新的工作階段：
  * 網頁靜置超過 30 分鐘
  * 過了晚上十二點 00:00

## **數據**

* 數據大概每 1 小時更新一次
* 「交易」的「來源/媒介」是以「使用者」最後的 UTM campaign source 來計算
  * 如果完成交易的工作階段沒有UTM source/medium，系統會把交易歸入「使用者」最後一個 UTM source/medium
* 不同「來源/媒介」的交易數量與 Google Analytics 可能不同
  * 因為我們沒有置入代碼前的數據，部份交易會被歸入 direct / none
  * 在GA上使用者的來源會保留較長時間，所以亦會造成數據不相同

{% content-ref url="shopping-behavior.md" %}
[shopping-behavior.md](shopping-behavior.md)
{% endcontent-ref %}

{% content-ref url="source-medium.md" %}
[source-medium.md](source-medium.md)
{% endcontent-ref %}

