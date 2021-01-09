# 有大佬配置过宝塔跨域的问题么。


http://www.daimaplus.com/index.php/archives/Nginx%E9%85%8D%E7%BD%AE%E8%B7%A8%E5%9F%9F%E8%AE%BF%E9%97%AE.html<br />
<br />
百度搜索一堆啊。

我的博客有 https://2demo.top/24.html

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353238&amp;ptid=758481" target="_blank"><font color="#999999">2life.top 发表于 2020-10-26 11:37</font></a></font><br />
我的博客有 https://2demo.top/24.html</blockquote></div><br />
在你博客看到了 但是有个不是很懂 add_header Access-Control-Allow-Origin $http_origin; 这一句$http_origin代表变量&nbsp;&nbsp;也就是域名&nbsp;&nbsp;我并没有看到你说在那个位置设置可跨域域名那么是否$http_origin可以直接换成* 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353540&amp;ptid=758481" target="_blank"><font color="#999999">Clever 发表于 2020-10-26 12:40</font></a></font><br />
在你博客看到了 但是有个不是很懂 add_header Access-Control-Allow-Origin $http_origin; 这一句$http_o ...</blockquote></div><br />
可以的，但是HTTPS有时候会调用不了HTTP，HTTP两个都可以，你自己试试就行了

跨域关宝塔什么事

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353607&amp;ptid=758481" target="_blank"><font color="#999999">88232128 发表于 2020-10-26 12:59</font></a></font><br />
跨域关宝塔什么事</blockquote></div><br />
可能我写的有问题、宝塔NGINX配置跨域

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353598&amp;ptid=758481" target="_blank"><font color="#999999">2life.top 发表于 2020-10-26 12:57</font></a></font><br />
可以的，但是HTTPS有时候会调用不了HTTP，HTTP两个都可以，你自己试试就行了 ...</blockquote></div><br />
我试试

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353774&amp;ptid=758481" target="_blank"><font color="#999999">Clever 发表于 2020-10-26 13:32</font></a></font><br />
可能我写的有问题、宝塔NGINX配置跨域</blockquote></div><br />
crossdomain.xml 不香？你配置跨域跟我N某人何干<img src="static/image/smiley/yct/003.gif" smilieid="50" border="0" alt="" />
