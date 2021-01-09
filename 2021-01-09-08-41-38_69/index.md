# Frp内网穿透反向代理后安卓手机无法安装客户端


<i class="pstatus"> 本帖最后由 xxwzdc 于 2020-10-28 00:09 编辑 </i><br />
<br />
VPS服务器已经设置好，感谢各位的提示，直接在安卓手机上安装frp客户端，手机已经root，用终端连接执行命令后提示：can't execute<img src="static/image/smiley/default/tongue.gif" smilieid="7" border="0" alt="" />ermission denied，不知道原因，哪位帮忙解答一下

帮顶，只会FRP的HTTP和TCP连接！<br />
<br />
<img src="static/image/smiley/default/mad.gif" smilieid="11" border="0" alt="" /><img src="static/image/smiley/default/mad.gif" smilieid="11" border="0" alt="" /><img src="static/image/smiley/default/mad.gif" smilieid="11" border="0" alt="" />

<i class="pstatus"> 本帖最后由 nat.ee 于 2020-10-27 23:10 编辑 </i><br />
<br />
手机装frp服务端？<br />
你是要用frp穿透到手机上的http？<br />
还是说在手机搭建frps服务端，然后nginx反代frps服务端的http或https，我只能跟你说ksweb的nginx缺少反代模块，行不通！别折腾了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9361820&amp;ptid=759195" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-27 23:08</font></a></font><br />
手机装frp服务端？<br />
你是要用frp穿透到手机上的http？<br />
还是说在手机搭建frps服务端，然后nginx反代frps服务 ...</blockquote></div><br />
手机装客户端，服务端装VPS上。缺少模块行不通就浪费时间了，谢谢

你报错倒是贴上来啊，。。。。

<div class="quote"><blockquote><font color="#999999">xxwzdc 发表于 2020-10-27 23:14</font><br />
<font color="#999999">手机装客户端，服务端装VPS上。缺少模块行不通就浪费时间了，谢谢</font></blockquote></div><br />
你手机装frp客户端，不用反代啊笨，<br />
ksweb 默认配置启动就行，frp客户端就穿透本地这个nginx端口，http模式 127.0.0.1就行。
