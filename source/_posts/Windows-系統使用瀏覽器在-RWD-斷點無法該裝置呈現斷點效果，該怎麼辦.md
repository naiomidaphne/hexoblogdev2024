---
title: Windows 系統使用瀏覽器在 RWD 斷點無法該裝置呈現斷點效果，該怎麼辦?
date: 2024-05-31 14:32:22
tags: 
- RWD 
- windows
- 前端
---



[Codepen 測試](https://codepen.io/DaphneShen/pen/OJYMKbP)

我的電腦是 Windows 11 的版本，而我的電腦 ( Chrome、Firefox、Windows Edge ) 瀏覽器們的 DevTools 皆在 992px 斷點時乖乖從三排區塊文字變成兩排區塊文字，但是在斷點 767px 時發生問題，它會變成在 766px 才會從兩排區塊文字變成滿版的區塊文字 ，奇怪的是其他人在同一份資料 ( VScode、Codepen ) 操作的情況下是可以在 767px 的斷點時乖乖變成滿版區塊文字。

操作影片：
[影片一](https://www.loom.com/share/c002e7c187164f428e4db3e28f3024c7)

[影片二](https://www.loom.com/share/510a07b60d4f45649c89175e4d241767?sid=8e21a12c-1e4f-4cae-a1da-5c5f3ff53d33)


### 解決方法:
將斷點 767px 改成 **767.99px** 畫面即可在該斷點成功呈現想要的效果

[參考文獻](https://stackoverflow.com/questions/40272679/bug-media-query-max-width-plus-windows-10)

[成功後的畫面效果](https://www.loom.com/share/5eeb6bfe7b0a4c8aad67cfa48cccf4cc?sid=f6dd3c47-413a-4928-8f80-58eb74e6db04)
[影片二](https://www.loom.com/share/510a07b60d4f45649c89175e4d241767?sid=8e21a12c-1e4f-4cae-a1da-5c5f3ff53d33)


### 解決方法:
將斷點 767px 改成 **767.99px** 畫面即可在該斷點成功呈現想要的效果

[參考文獻](https://stackoverflow.com/questions/40272679/bug-media-query-max-width-plus-windows-10)

[成功後的畫面效果](https://www.loom.com/share/5eeb6bfe7b0a4c8aad67cfa48cccf4cc?sid=f6dd3c47-413a-4928-8f80-58eb74e6db04)