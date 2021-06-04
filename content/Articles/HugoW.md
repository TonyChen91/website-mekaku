---
title: "教學: 如何使用Hugo在Github部署網站?"
date: 2021-06-04T16:19:20+08:00
draft: false
author: "Tony"
categories: ["手札"]
tags: ["程式"]
image: "https://chupai.github.io/images/covers/200316_hugo.png"
---
**{{< mh 28 >}}{{< mcolor	palevioletred>}}什麼是GitHub和GitHub Page{{< /mcolor >}}{{</mh>}}**
***
\
在介紹Github和Github Pages之前，先介紹一下網頁的種類以及網址。  
\
網頁有分動態和靜態:   
\
**\- 動態網頁:** 及時與讀者互動，像是YT、FB這種網頁屬於此種。  
有會員功能、購物車、討論區...等。通常使用Perl、PHP、ASP、JSP、ColdFusion來寫程式     
\
**\- 靜態網頁:** 不方便管理、易搜尋、較簡單設計和上手。通常是用HTML、CSS、JavaScript來編寫。  
\
要架設網站，除了網頁設計，還有網址的問題。  
網址是連結網站的一個窗口，同一個網站的不同頁面，也都是不同網址所構成。   
\
那問題來了，網址該如何取得?   
通常愈簡單的網址愈容易讓使用者記住，也都愈容易。   
不幸的是，自訂網址是要收錢的，而且不是永久。    
但你也很幸運，本文將教你如何**免費**設立網頁和網址。    
\
\
回歸正題，什麼是Github和Github Pages??  
**\- GitHub: 存放程式碼/公開代原碼的平台，任何人都可以訪問。   
\- Github-Pages: 利用你在GitHub放的資料來架設網站。**  
\
\
簡單來說，你把網頁上傳到GitHub，並命名特定的名稱，  
接著GitHub-Pages會自動把這個特定名稱的整個儲存庫(repo)給放上特定的網址。  
任何訪問該網址的人，會去...         
首先先去看看[Github Pages](https://pages.github.com/)的介紹     
\
**{{< mh 28 >}}{{< mcolor	palevioletred>}}什麼是Hugo{{< /mcolor >}}{{</mh>}}**
***
\
\
**{{< mh 28 >}}{{< mcolor	palevioletred>}}步驟一:安裝Hugo註冊Github{{< /mcolor >}}{{</mh>}}**
***
\
\
**{{< mh 28 >}}{{< mcolor	palevioletred>}}步驟二:了解Hugo架構{{< /mcolor >}}{{</mh>}}**
***
\
看一下你的網站的草稿:
```html
hugo server
<!--在自己的電腦執行網站的草稿-->
```  
\
接著你就可以在 localhost:1313 這個網址上看到大致上的模板。  
\
最後將這些文章.程式.圖片檔等打包進public的資料夾
```cmd
hugo
```
\
**{{< mh 28 >}}{{< mcolor	palevioletred>}}步驟三:上傳至GitHub{{< /mcolor >}}{{</mh>}}**
***
打開你的命令提示字元(cmd)，或者你用其他軟體打開也可。
記得先鎖定位置到/public這個資料夾後在進行以下步驟:
\
\
Step1:
```html
git add .
<!--代表把所有檔案加入暫存區-->
```  
\
Step2:
```html
git commit -m "Version 1.0"
<!--確認進入待上傳區-->
<!---m "XXX" 的意思是給這次上傳到GitHub的檔案一條訊息，隨便寫也可-->
```  
\
Step3:
```html
git push -u origin master
<!--代表把所有檔案加入暫存區-->
```  
