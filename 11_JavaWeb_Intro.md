# JavaWeb Intro

## 基本概念
- web开发：**在java中，动态web资源开发的技术成为JavaWeb**
    - 静态: html, css
    - 动态
    - 技术栈：Servlet/JSP, ASP, PHP
## web应用程序: 可以提供浏览器访问的程序
- a.html, b.html....多个web资源，这些web资源可以被外界访问，对外界提供服务
- 能访问到的哦任何一个页面或者资源，都存在于某个计算机上
- url
- 这个合格统一的web资源会被放在同一个文件夹下, web应用程序-->Tomecat:服务器
- 一个web应用由多部分组成（静态web，动态web）
    - html, css, js
    - jsp, servlet
    - Java 程序
    - jar包
    - 配置文件(Properties)
web应用程序编写完毕后，若想提供给外界访问: 需要一个服务器来统一管理

## 静态 web
- *.htm, *.html 这些都是网页的后缀. 如果服务器上一直存在这些东西，我们就可以进行读取
- 缺点：
    - web页面无法动态更新,所有用户看到的都是同一个页面
        - 伪动态：实际开发中，经常用JavaScript。让静态网页动起来
    - 无法和数据库交互(数据无法持久化,用户无法交互)
![05](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/05_JavaWeb.png)