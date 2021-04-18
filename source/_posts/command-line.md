---
title: command-line 指令
date: 2021-04-12 21:20:39
categories: command-line
tags:
  - command
  - 鋰學院第五屆計畫
---
## 使用cmd
下載git 使用其git-bash
<!-- more -->
## 指令

| 指令 | 說明 | 例子 |
|:-:|:-:|:-:|
|pwd(cd)|查看目前位置|`pwd`|
|ls(dir -l)|顯示檔案|`ls -al`|
|cd|選擇檔案|`cd work` (進到work資料夾)|
|help|查詢指令功能|`help cd` (Ms限定)|
|touch|建立檔案or更改時間|`touch 123`(沒有123則新增，反之更改成現在時間)|
|rm(del)|刪除檔案|`rm 123`(刪除123檔)<br>`rm -r 1234`(刪除1234資料夾)|
|mkdir(md)|新增資料夾|`mkdir 1234`|
|mv(ren)|移動檔案或改名|`mv 123 1234`(有1234資料夾則移動至夾內，反之123檔名變成1234)|
|cp(copy)|複製|`cp 123 1234`(複製123檔成1234檔)|
|vim|文字編輯器|vim 123(編輯123檔)<br>`i` 撰寫模式 `Esc`鎖定 `:q`不儲存離開 `:wq`儲存離開|
|cat|叫出文本內容|`cat 123`|
|grep|抓取關鍵字|`grep o 123` 找尋123中的o(git-brah不會反紅)|
|> <br> >> <br> echo|加入文本入檔|`ls 123 >1234`打印123的內容輸入1234中 <br>`echo "1234" > 1234`把1234(字元)**覆蓋**1234檔中所有內容<br>`echo "hello world" >> 1234`把hello world(字元)**增加**1234檔中所有內容 |
|curl|顯示回傳respond|`curl 網址` <br>`curl -s 網址` (隱藏進度條)顯示回傳respond|
|grep|搜尋關鍵字|grep 關鍵字 尋找位置 <br>ex. grep name /bin 找到尋找位置裡的關鍵字<br>grep -n 顯示關鍵字所在的行數|
|awk|以欄為單位數據處理|awk 'BEGIN {FS=":"} {print $3}'<br>FS代表目前的分隔字元，預設是空白鍵<br>print為把某欄東西列出來，範例為第三欄<br>BEGIN代表著先執行以下，像是這個範例是先執行 {FS=":"}，才找到$3打印|
|sed|串流編輯|s:取代 sed 's/have/had/1<br>#把每行第一個have取代成had|
<!-- | `|` |連結| `cat 1234 | grep o` 打開文本內容並找尋其含有o的字句| -->