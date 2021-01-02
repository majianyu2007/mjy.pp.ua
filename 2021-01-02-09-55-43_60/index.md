# 救救孩子怎么写python自动签到脚本


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349224&amp;ptid=758225" target="_blank"><font color="#999999">bert 发表于 2020-10-25 11:43</font></a></font><br />
抓了，但是用包里没有点击的value</blockquote></div><br />
你得签到才有post

不用考虑选择地区。点击按钮啥的，只要f12网络。你点击签到的那个请求用python发包就行。一般签到就一个请求。你只要知道提交的地址。和需要的参数就行。。。你可以参考别的脚本看看。都一个原理

F12或者抓包，找到签到的那个post链接就行了<img id="aimg_YZaDu" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

哪个网站的签到，这么复杂

贴出你的网址<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

学会正则就行

要么找到你想签到的链接去post&nbsp;&nbsp;form，要么用selenium模拟浏览器点击

网站贴出来

网址贴出来 看看~<br />
还有就是你的python代码也贴出来~~

直接看请求的地址和参数，抓包下来，然后每天定时post执行<br />
这个应该有按钮监听，看看JS那段Ajax也可以
