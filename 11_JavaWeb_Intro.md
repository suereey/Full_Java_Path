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

## 动态Web
- 页面会动态展示。 web的页面展示效果因人而异
- 缺点：
    - 假如服务器外部的web资源出现了错误，我们需要重新编写我们的后台程序,重新发布
        - 停机维护
- 优点:
    - 可以动态更新，所有用户看到的都不一样
    - 可以与数据库交互
![06](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/06_JavaWeb.png)

## web服务器
- 技术
    - ASP (not important now): 
        - microsfoft
        - 在html中嵌入了vb的脚本，ASP+COM
        - 在ASP开发中基本一个页面都有几千行业务代码，页面乱。维护成本高

    - PHP (more popular)
        - 开发速度快，功能强大，跨平台，代码简单 (70%, WP)
        - 无法承载大访问量的情况（局限性）

    - **JSP/Servlet**:
        - Sun公司主推的B/S架构
            - B/S浏览器和服务器
            - C/S客户端和服务器
        - 基于java
        - 可以承载三高问题带来的影响

- **web服务器: 服务器是一种被动的操作，用来处理用户的一些请求和给用户一些相应信息**
    - **Tomcat** 实际上运行JSP 页面和Servlet

## Tomcat
- Install Tomcat
- 启动和配置
    ![14_tomcat](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/14_TomCat_install.png)
    - start: apache-tomcat-10.0.22-windows-x64\apache-tomcat-10.0.22\bin\startup.bat
    - **http://localhost:8080/**
    - close
- Related ports:
    - tomcat: 8080
    - mysql: 3306
    - http: 80
    - https: 443
- 网站是如何访问的?
    - 输入一个域名：回车
    - 检查本机的C:\WINDOWS\system32\drivers\etc\hosts配置文件下有没有这个域名的映射
        - Yes: 直接返回ip地址，这个地址中，有我们需要访问的web程序
        ```127.0.0.1    www.xxx.com```
        - No: 去DNS服务器找. (DNS: 全世界的域名都在这管理)

