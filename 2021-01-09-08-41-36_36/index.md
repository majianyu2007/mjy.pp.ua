# 网站首页，列表页，都正常，内容页国外打开正常，国内502


首页&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ……<font color="SeaGreen">OK</font><br />
列表页&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ……<font color="SeaGreen">OK</font><br />
内容页<font color="DarkOrange">国内</font>&nbsp; &nbsp; &nbsp; &nbsp; ……<font color="Red">502 Bad Gateway</font><br />
内容页国外&nbsp; &nbsp; &nbsp; &nbsp; ……<font color="SeaGreen">OK</font><br />
<br />
<br />
<br />
<br />
求教大佬，这是咋回事？难道被G-F-W墙了内容页？但是闻所未闻啊？有<strong>只墙内容页</strong>这样的情况吗？

UP

不懂 帮顶&nbsp; &nbsp;&nbsp;&nbsp;<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

502不是你自己server的问题？HTTPS 能算到 高墙 上去？

502是被墙嘛？<br />
<br />
好像不是吧！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359563&amp;ptid=759010" target="_blank"><font color="#999999">iks 发表于 2020-10-27 15:32</font></a></font><br />
502不是你自己server的问题？HTTPS 能算到 高墙 上去？</blockquote></div><br />
问题是为什么我在国外服务器上访问是可以的呢？我有点想不明白这个

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359582&amp;ptid=759010" target="_blank"><font color="#999999">BQQ 发表于 2020-10-27 15:34</font></a></font><br />
问题是为什么我在国外服务器上访问是可以的呢？我有点想不明白这个</blockquote></div><br />
从防火墙或 nginx 层和 php 层找问题

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359593&amp;ptid=759010" target="_blank"><font color="#999999">iks 发表于 2020-10-27 15:36</font></a></font><br />
从防火墙或 nginx 层和 php 层找问题</blockquote></div><br />
<br />
国外服务器上用chrome浏览器随便访问一个内容页是正常的，然后，我用无痕模式访问，果然也是502了<br />
<br />
MD,果然还是自己服务器或者网站有问题

曾经遇到同样的问题。。。我把nginx版本降低了。。就好了

502,查日志找
