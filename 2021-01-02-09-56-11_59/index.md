# 宝塔国际版（aaPanel）会收集哪些信息，附官方解释


<i class="pstatus"> 本帖最后由 fullbody 于 2020-11-5 22:20 编辑 </i><br />
<br />
关于aaPanel安装脚本的跟踪代码：<br />
1.当用户安装面板时，安装脚本的跟踪代码用于记录服务器IP，安装时间和该IP的安装次数。脚本代码在安装过程中只会记录一次<br />
2.ajax.py中的代码将收集用户ip，站点总数，数据库和ftp总数，设备信息（系统版本，内存大小，处理器型号，Web服务器类型，面板版本）<br />
3.ajax.py还有一个代码可以记录IP是否在此处安装aaPanel<br />
<br />
原文：https://forum.aapanel.com/d/1504-about-the-tracking-code-of-the-aapanel-installation-script<br />
其他：https://www.lowendtalk.com/discussion/comment/3105526#Comment_3105526<br />
<br />
至于国内版宝塔面板会收集哪些信息就不得而知了。希望有测试过的大佬能说下。<br />
毕竟由于监管的不同，很多软件的国内国际版都区分对待

<i class="pstatus"> 本帖最后由 fullbody 于 2020-11-6 11:01 编辑 </i><br />
<br />
其实当你用浏览器打开宝塔面板的登录页面时，<br />
页面默认会加载宝塔APP的图片，<div class="blockcode"><div id="code_tee"><ol><li>http://app.bt.cn/static/app.png</ol></div><em onclick="copycode($('code_tee'));">复制代码</em></div><br />
理论上，就已可以通过浏览器的请求头Referer记录到了用户登录IP，服务器IP，面板端口，安全入口和其他信息，不过这些都在他的网站日志里。<br /><div class="blockcode"><div id="code_BWb"><ol><li>Referer: http://XXX.XXX.XXX.XXX:8888/xsdwdwdd/</ol></div><em onclick="copycode($('code_BWb'));">复制代码</em></div><br />
<br />
国内版国外版都有此情况，打算用aaPanel的注意一下。<br />
可以用浏览器插件伪装Referer和X-Forwarded-For<br />
<br />
注意：ModHeader被爆有安全问题

<i class="pstatus"> 本帖最后由 fullbody 于 2020-11-5 22:24 编辑 </i><br />
<br />
另外看源码发现宝塔国内版某个文件夹下有大量伪装成图片的代码，<br />
不知这样搞有何意义？<br />
好像是宝塔首页的源码？<br />
/www/server/panel/BTPanel/static/img/dep_ico/目录下<br />
bfz.png<br />
JTBC.png<br />
skm.png<br />
test.png<br />
test2.png<br />
ttttt.png<br />
wp.png<br />
z-blog.png<br />
ZFAKA.png<br />


<i class="pstatus"> 本帖最后由 ezreal 于 2020-11-5 14:19 编辑 </i><br />
<br />
很简单，如果官方想做坏事。你IP有了，管理端口一般是默认的。如果有后门的话，那不是为所欲为了。<br />
如果不收集IP，即使有后门，也不知道哪个IP装了BT。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9408976&amp;ptid=762727" target="_blank"><font color="#999999">fullbody 发表于 2020-11-5 21:52</font></a></font><br />
其实当你用浏览器打开宝塔面板的登录页面时，<br />
页面默认会加载宝塔APP的图片，<br />
理论上，就已可以通过浏览器 ...</blockquote></div><br />
注意！！！最近 Chrome 应用商店安装量最高的 ModHeader 扩展爆出问题了<br />
<br />
贴个大佬的分析笔记<br />
https://blog.berd.moe/archives/chrome-malware-extension-modheader/<img id="aimg_yx0I9" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

居然收集这么多信息。。。。。。

利用闲时挖币

问题是，收集来干嘛？收集时提示用户同意了没？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9405908&amp;ptid=762727" target="_blank"><font color="#999999">krazy176 发表于 2020-11-5 12:02</font></a></font><br />
居然收集这么多信息。。。。。。</blockquote></div><br />
这还是英文版的，<br />
国内版估计收集得更多

看来我只能用lnmp了吗?

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9405905&amp;ptid=762727" target="_blank"><font color="#999999">h20 发表于 2020-11-5 12:02</font></a></font><br />
问题是，收集来干嘛？收集时提示用户同意了没？</blockquote></div><br />
原文中管理员解释得最后得一段话：<br />
“除此之外，我们没有其他跟踪代码。如果以后需要跟踪任何信息，我们将在此处添加一条语句，并在用户同意后执行跟踪。<br />
<br />
最后，感谢您的信任和使用”

看了一下，国内版这几处代码也存在

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9406485&amp;ptid=762727" target="_blank"><font color="#999999">ezreal 发表于 2020-11-5 14:09</font></a></font><br />
很简单，如果官方想做坏事。你IP有了，管理端口一般是默认的。如果有后门的话，那不是为所欲为了。<br />
如果不 ...</blockquote></div><br />
有些道理
