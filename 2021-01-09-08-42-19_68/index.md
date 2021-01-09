# wordpress更新后卡登录界面了


<br />
<br />
昨晚收到邮件说自动升级了版本<br />
<br />
<br />
结果今天登录不了后台了(循环卡在登录界面)<br />
<br />
<br />
倒也不敢完全肯定是升级了版本的问题，不过这期间好像也没发生别的事了<br />
<br />
<br />
有点难受<br />
<br />
<br />
<img id="aimg_XE2OK" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://developer-forum-online.cdn.bcebos.com/cfb3ff5a-6301-4c4b-ad8f-115921583cf6.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />


把后台插件删掉 然后进去后在恢复一下就行了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9384440&amp;ptid=760919" target="_blank"><font color="#999999">周润发 发表于 2020-11-1 12:25</font></a></font><br />
把后台插件删掉 然后进去后在恢复一下就行了</blockquote></div><br />
后台插件是指？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9384442&amp;ptid=760919" target="_blank"><font color="#999999">嗷嗷 发表于 2020-11-1 12:26</font></a></font><br />
后台插件是指？</blockquote></div><br />
去 wp-content/plugins 把插件文件夹名修改，一个一个试，然后访问后台试试

自动升级倒是没卡，不过5.5到现在也没中文语言，你升的这个？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9384473&amp;ptid=760919" target="_blank"><font color="#999999">胖虎 发表于 2020-11-1 12:34</font></a></font><br />
自动升级倒是没卡，不过5.5到现在也没中文语言，你升的这个？</blockquote></div><br />
不是5.5，连着两天升级了，现在是5.4.4<br />
<img id="aimg_rF8Au" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://developer-forum-online.cdn.bcebos.com/ac4eb893-339a-44bf-ae0f-79edaabf2bb2.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

为什么我的都5.5.1了

早就锁定了版本不让他自动更新了…

<i class="pstatus"> 本帖最后由 爱吃醋的醋醋 于 2020-11-1 13:22 编辑 </i><br />
<br />
明显是插件的锅，这关wp什么事情，还有wp最新版是5.5.3

我的都5.53了，没发现这样的问题
