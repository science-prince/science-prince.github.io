---
title: "用linux下常用命令wget进行整站下载（递归下载至本地）"
categories: linux
tags: wget website download curl
---

这个命令可以以递归的方式下载整站，并可以将下载的页面中的链接转换为本地链接。 

wget加上参数之后，即可成为相当强大的下载工具。 
```
wget -r -p -np -k http://xxx.com/abc/
```
 
```
-r,  --recursive（递归）          specify recursive download.（指定递归下载） 
-k,  --convert-links（转换链接）      make links in downloaded HTML point to local files.（将下载的HTML页面中的链接转换为相对链接即本地链接） 
-p,  --page-requisites（页面必需元素）    get all images, etc. needed to display HTML page.（下载所有的图片等页面显示所需的内容） 
-np, --no-parent（不追溯至父级）          don't ascend to the parent directory. 

另外断点续传用-nc参数 日志 用-o参数 
```