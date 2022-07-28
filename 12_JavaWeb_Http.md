# Http
## What is Http: 超文本传输协议
- http: 是一个简单的请求－响应协议，它通常运行在TCP之上
    - 文本： html, 字符串
    - 超文本：图片，音乐，视频，定位，地图
    - port: 80
    - https port: 443
- 两个时代
    - http1.0: 
        - HTTP/1.0: 客户端可以与web服务器连接后，只能获得一个web资源. 断开连接

    - http2.0: 
        - HTTP/1.1: 客户端可以与web服务器连接后，可以获得多个web资源

## http请求 request
![15](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/15_request.png)

Request Body
- request method： GET， POST， PUT， DELETE
    - GET: 请求能够携带的参数少，大小有限，会在浏览器的url地址栏显示数据内容，不安全，但高效
    - PUT: 请求能够携带的参数没有限制，大小没有限制，不会在浏览器的url地址栏显示数据内容，安全，但不高效 (not no difference in 5G internet)

Request Head
![18_requesthead]()




## http响应 response
![16](https://raw.githubusercontent.com/suereey/Full_Java_Path/main/ScreenShot/JavaSE/16_response.png)

Response code:
- 200： 请求响应成功
- 3××：请求重定向
- 404：找不到资源
- 4**: 资源不存在
- 5**: 服务器代码错误

# Maven