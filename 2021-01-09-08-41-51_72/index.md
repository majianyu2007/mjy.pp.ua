# virmach 重装centos 7后，一直报/var/run/yum.pid: another copy is running


<br />
virmach 重装centos 7后，想装软件<br />
<br />
一直报<br /><div class="blockcode"><div id="code_kAu"><ol><li>ck /var/run/yum.pid: another copy is running as pid 867.<br /><li>Another app is currently holding the yum lock; waiting for it to exit...<br /><li>&nbsp;&nbsp;The other application is: yum<br /><li>&nbsp; &nbsp; Memory :&nbsp; &nbsp; 0&nbsp;&nbsp;RSS (997 MB VSZ)<br /><li>&nbsp; &nbsp; Started: Wed Oct 28 20:53:55 2020 - 05:24 ago<br /><li>&nbsp; &nbsp; State&nbsp;&nbsp;: Sleeping, pid: 867<br /><li>Another app is currently holding the yum lock; waiting for it to exit...<br /><li>&nbsp;&nbsp;The other application is: yum<br /><li>&nbsp; &nbsp; Memory :&nbsp; &nbsp; 0&nbsp;&nbsp;RSS (997 MB VSZ)<br /><li>&nbsp; &nbsp; Started: Wed Oct 28 20:53:55 2020 - 05:26 ago<br /><li>&nbsp; &nbsp; State&nbsp;&nbsp;: Sleeping, pid: 867</ol></div><em onclick="copycode($('code_kAu'));">复制代码</em></div><br />
<br />
<br />
昨天尝试网上的强制结束，<br />
rm -f /var/run/yum.pid<br />
结果系统好像有问题<br />
<br />
<br />
请问是重装后，系统在更新么<br />


这个版本 <br />
<br />
CentOS 7 x86_64 Minimal v2<br />
<br />
CentOS is an Enterprise-class Linux Distribution derived from sources freely provided to the public by a prominent North American Enterprise Linux vendor. CentOS conforms fully with the upstream vendor's redistribution policy and aims to be 100% binary compatible. (CentOS mainly changes packages to remove upstream vendor branding and artwork.) CentOS is free.

vir家系统装完会自己yum upgrade。等几分钟它自己重启完就好了<img id="aimg_vHU7S" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367563&amp;ptid=759667" target="_blank"><font color="#999999">QEMU 发表于 2020-10-29 09:15</font></a></font><br />
vir家系统装完会自己yum upgrade。等几分钟它自己重启完就好了</blockquote></div><br />
等了大概10分钟，已经重启了，好了。<br />
谢谢老板

重启**好
