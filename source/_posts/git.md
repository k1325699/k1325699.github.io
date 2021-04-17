---
title: git & github
date: 2021-04-13 21:37:06
categories: git
tags:
 - git
 - github
 - - 鋰學院第五屆計畫
---
## git基礎指令


### git init
 建立git
<!-- more -->
### git status
顯示目前git狀態(已上傳、未上傳、修改為上傳的檔案)

### git add

將新增的檔案傳至版本控管

```
git add 123 (將123檔案加至控管當中)
git add .(將資料夾中的所有檔案加入控管當中)

git add -A
git add --all 把所有專案的內容放進控管

```

### git commit

上傳成新版本

```
git commit -am "說明"(上傳更改與加入控管的新檔案成新版本)
```

### git log

顯示所有更改的版本

### git checkout

```
git checkout 版本名稱 回歸(此名稱的)版本
git checkout 分支 移動到分支
```

### .girignore

把不做版控的檔案放置裡面

## 分支

### git branch

```
git branch 123 建立名為123的分支

git branch -v 顯示所有分支與現在所在分支

git branch -d 123 刪除名為123的分支
```

### git merge

```
git merge 123 在a(目前)分支當中把123合併進去
```

### 錯亂

### git push

```
git push origin a 把git放入github中的a分支
```

### git pull

```
git pull origin a 把github中的a分支放入git中
```

### git clone 

```
git clone 網址 從網址的檔案下載下來
```

### git diff

```
git diff 檔案 觀看更改內容
```

## 情境

### commit後想改commit message

```
git commit --amend 跑出編輯器可更改message
```

### commit後不想commit

```
git reset head^
預設為--mixed(git reset head^--mixed) 回歸前一個版本，更改內容並沒有上傳版控 
--soft 回歸前一個版本，更改內容並上傳至版控
--hard 回歸前一個版本，刪除更改內容
```

### 還沒commit但改的東西不想要

```
git checkout -- 檔案名稱 回到檔案之前的內容
```

### 更改branch名稱

```
git branch -m 更改名稱
```