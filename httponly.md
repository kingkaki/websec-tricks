HttpOnly利用总结
https://www.t00ls.net/viewthread.php?tid=48122
1、协议TRACE方法
2、中间件 apache squid报错泄露
3、页面链接，比如phpinfo泄露cookie，url链接(可能带用户名密码或者cookie)，功能页面（找某种写入到网页里面的凭证）。
4、接口获取token其他敏感信息
5、其他子域名或者第三方网站
6、获取网站html进行csrf
7、进行钓鱼

httponly
利用squid轻松获取经http only保护的cookie内容 wooyun-2013-025343
http://wooyun.jozxing.cc/static/bugs/wooyun-2013-025343.html
中间件报错

知乎某中间件配置不当 导致httponly保护的COOKIE泄露 wooyun-2013-037312
http://wooyun.jozxing.cc/static/bugs/wooyun-2013-037312.html
中间件报错

新浪微博某漏洞修复不当可XSS/盗取用户httponly cookie wooyun-2016-0191864
https://wy.tuisec.win/wooyun-2016-0191864.html
代理

通过一糯米XSS可绕chrome并可用两种方式拿到httponly的BDUSS（大部分非IE用户点击后百度云盘资料会被泄露） wooyun-2015-0133351
https://wy.tuisec.win/wooyun-2015-0133351.html
第三方网站 接口

百度任意XSS绕过HTTPONLY BDUSS wooyun-2015-099935
https://wy.tuisec.win/wooyun-2015-099935.html
二级域名

apache httponly bypass
利用apache server head limit 8192字节限制, 从400状态页爆出httponly保护的cookie
中间件报错