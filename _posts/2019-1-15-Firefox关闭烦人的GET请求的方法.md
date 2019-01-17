### Firefox关闭GET请求到detectportal.firefox.com网站的方法

每次用Firefox挂代理抓包，就会发现浏览器每几秒就自动发个GET请求包到`http://detectportal.firefox.com/success.txt`<br>

真的是神烦，每次都污染burp的HTTP history<br>

google了一下，方法如下：<br>

1. 地址栏输入`about:config`<br>
2. 搜索`network.captive-portal-service.enabled`<br>
3. 双击选项改为false就行了<br>

从此之后，世界清净了~