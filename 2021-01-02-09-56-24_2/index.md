# 关于网站套cdn之后 无法禁止某些ip访问网站的问题


我网站套了cdn加速&nbsp;&nbsp;然后现在宝塔无法获取到访问用户真实的ip, Nginx也无法获取到<br />
<br />
有的人会说,可以用第三方例如百度统计来看到啊!<br />
<br />
这样确实可以,但是只是你知道,宝塔并不知道,宝塔不知道也就是说你在宝塔里面设置封禁某些ip的时候&nbsp;&nbsp;其实是没用的 因为用户是通过cdn访问的,<br />
所以必须要获取到真实的ip<br />
<br />
但是我通过网上的帖子尝试了 还是不行 <br />
我套了两层cdn 一个小厂的和一个cf<br />
<br />
现在就是无法获取真实ip 球大佬帮忙<br />
<br />
<br />
https://rcwap.com/newsdetail_135.html

请技术大佬们回答吧！<br />
<br />
我帮楼主谢谢了！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

看header能不能把真实ip传过来<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><br />
还有看你先套的哪个cdn

那就直接在服务器上用iptables禁掉吧

这个方法一层CDN好像可以。<br />
二层的弄这么严实 再加了反代么

这需要你的CDN把IP传过来 哈哈哈

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9450853&amp;ptid=766414" target="_blank"><font color="#999999">liuyangge 发表于 2020-11-13 22:33</font></a></font><br />
看header能不能把真实ip传过来<br />
还有看你先套的哪个cdn</blockquote></div><br />
header在哪看&nbsp;&nbsp;<br />
第一层是cf&nbsp;&nbsp;第二层是买的小厂的

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9450858&amp;ptid=766414" target="_blank"><font color="#999999">juzi5914 发表于 2020-11-13 22:34</font></a></font><br />
那就直接在服务器上用iptables禁掉吧</blockquote></div><br />
这个方法可以绕过cdn 直接禁真实用户ip吗

HTTP_X_FORWARDED_FOR<img id="aimg_AxrTd" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9450871&amp;ptid=766414" target="_blank"><font color="#999999">tir 发表于 2020-11-13 22:37</font></a></font><br />
这需要你的CDN把IP传过来 哈哈哈</blockquote></div><br />
这个需要你的 cdn支持才可以是吧&nbsp;&nbsp;要在cdn的控制面板里面设置吗
