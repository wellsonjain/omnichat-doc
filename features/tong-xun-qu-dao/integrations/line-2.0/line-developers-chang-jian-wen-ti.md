# LINE Developers 常見問題

#### Q： 我從  LINE Official Account Manager（Line OA 後台）->「設定」-> 「Messaging API」-> 點擊 「LINE Developers」 進入，但我沒有看到底下畫面

A：如果您進入並登入自己的 LINE 帳號後，出現以下畫面，表示您沒有該 LINE 帳號的 Provider 和 Messaging API Channel 管理員 Admin 權限。\
請洽詢貴司同仁是否之前創建過 Messaging API Channel 並按照該路徑進入。如果找不到創建同仁，請與 LINE 官方客服聯繫取回帳號權限

![](<../../../../.gitbook/assets/截圖 2022-03-31 下午12.45.24.png>)

#### Q：Login channel 一定要跟 Messaging API Channel 在同一個 Provider 內嗎？

A：一定的。因為 LINE 官方規定兩個 Channel 需在同一個 Provider 底下才能進行觸發相關功能

#### Q：如果找不到 Messaging API Channel，我可以自己重新創建一個嗎？

A：不行。每一個 LINE 官方帳號都只有一個 Messaging API Channel，無法重新創建一個。如果您找尋不到 Messaging API Channel 和所屬 Provider 權限，請與 LINE 官方客服聯繫取回帳號權限

#### Q：如果其他同仁找到 Messaging API Chanel，請問要怎麼授權給其他人？

A：可以使用 E-mail 授權給其他人，請參考下方做法。先將該 Provider 進行授權，接著點擊進 Messaging API Channel 一樣 E-mail 操作

{% hint style="info" %}
1. 如用 E-mail 授權給其他同仁，無法撤回授權信件
2. 登入 E-mail 拿到 Provider / Channel 授權時，請確認登入的帳號（LINE 個人帳號或是 E-mail ）
3. 無法刪除當時創建 Messaging API Channel 的人員帳號
{% endhint %}

![Provider 內按下「Role」](<../../../../.gitbook/assets/截圖 2022-03-31 下午2.45.02.png>) ![進到 Role 內按照以下步驟](<../../../../.gitbook/assets/截圖 2022-03-31 下午2.45.54.png>)

先在 Provider 內按下「Role」

1. Invite by email
2. 輸入您要授權的同仁
3. 選擇權限角色，需為 Admin 管理員才能做後續步驟
4. 送出邀請

![在 Messaging API Channel 內權限](<../../../../.gitbook/assets/截圖 2022-03-31 下午2.52.56.png>)

#### Q：我按照下方方式創建 Login Channel 為什麼無法連動 LINE OA 帳號或是無法使用？

A：請先確認您創建的 Login Channel 是否與 Messaging API Channel 在同一個 Provider 內（如下圖）如未看到類似畫面或是沒有看到 Messaging API Channel，請回到 LINE Developers 常見問題第一題確認權限。

#### Q：請問我在 Omnichat 後台看到有遊戲模組 LIFF 跟社群身份綁定 LIFF，可以使用相同的 LIFF ID 嗎？

A：不可以。Login channel 可以使用同一個，但 LIFF 必須要分開建立。因為 Endpoint URL 的顯示是完全不一樣的唷！

關於遊戲模組 LIFF 設定

{% content-ref url="you-xi-mo-zu-zhuan-yong-line-liff-id-she-ding.md" %}
[you-xi-mo-zu-zhuan-yong-line-liff-id-she-ding.md](you-xi-mo-zu-zhuan-yong-line-liff-id-she-ding.md)
{% endcontent-ref %}

關於社群身份綁定 LIFF 設定

{% content-ref url="she-qun-shen-fen-bang-ding-liff-she-ding.md" %}
[she-qun-shen-fen-bang-ding-liff-she-ding.md](she-qun-shen-fen-bang-ding-liff-she-ding.md)
{% endcontent-ref %}
