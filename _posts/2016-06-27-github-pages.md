---
layout: post
title:  "Github pages"
date:   2016-06-27 
thumb: http://moduslaborandi.net/wp-content/uploads/2015/05/github.pages.jpg
categories: jekyll 
---


>這裡是用GitHub pages+Jekyll搭建的靜態網頁  
因為單純想要做學習日誌，沒有需要會員、採購、後端管理...等需要資料庫的系統，
再加上想開始嘗試使用GitHub，所以選擇了這個搭建方式。

不管有多少教學文都聲稱搭建有多簡單，但還是被折騰到了!!  
所以列出過程中的注意事項以避免再做一次而犯錯卡關:

* 在看任何教學前先看發文日期  
不管寫得有多詳盡，這領域的變動速度實在太快，更新和修正後的狀況不一定和搭建時的一樣。

* User or organization site V.S Project site   
是不一樣的!!我是到後來搭建完才發現，這也是為什麼看很多教學有時候會讓我搞混。  

 User or organization site 的 URL: `http(s)://<username>.github.io`  
 Project site 的 URL: `http(s)://<username>.github.io/<projectname>`
 
詳細差異可參考[此篇](http://wiki.jikexueyuan.com/project/github-pages-basics/)介紹
 
* 自動生成 vs 手動創建  
標題寫快速搭建的文章有些都是github自動生成的版面，當然快，
可是因事先沒分清楚差別，如果不是自己想要的方式，反而花了不少爬文時間。  
要先決定使用github自動產生的模板或是Jekyll的模板，兩種文件都在github上，會一直顯現不出jekyll的模組。

* Github使用方式  
若是中文的教學，還是以簡體中文的比例較多，因為中國還需要翻牆，所以在使用這類型的工具上會多了一些步驟，要注意哪些其實我們根本可以略過。
[連猴子都能懂得Git入門指南](http://backlogtool.com/git-guide/tw/)，名字取的很好的網站!!  
~"~因為不想輸給猴子，所以會想認真看!! 

* Markdown語法    
不太複雜可以做中學，但是從別人的樣板對照出現的效果去記憶會事半功倍。
`檔名不可寫中文，否則內文也會顯示亂碼`

* Jekyll   
Theme如何套用呢?  
對程式碼小白來說，最熟悉的是檔案管理員而不是command-line，找到相對應的文件複製貼上也是可以的。

* _config配置    
很重要很重要，很多版型套用上去後效果沒有出現，原來是配置時沒有寫上。

* _site    
剛開始的時候我連_site都複製，後來看到英文教學才知道其實這是不能碰的。
網站生成後，最終的檔案都會放進這個資料夾，可以先把它清空，之後jekyll serve資料夾就會出現生成的內容。

* 插入本機圖片 
  
	`![]file:/// 文件的絕對路徑`
	
* 字型  
使用google的webfont，不知為何@import一直失敗，後來貼整陀google給的css，讓檔案少了request的過程才成功。   

以上是我過程中有卡關的幾個點，分享[這個](http://playingfingers.com/2016/03/26/build-a-blog/)我覺得較完整的教學
