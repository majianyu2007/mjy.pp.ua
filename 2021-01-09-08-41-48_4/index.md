# 腾讯云香港轻量。宝塔装了系统防火墙后打不开了


腾讯云香港轻量。<br />
宝塔装了 系统防火墙 后宝塔和网站打不开了<br />
<br />
系统防火墙啥也没设置，只点了启动就掉线了。。。<br />
<br />
咋进宝塔删宝塔的防火墙啊<br />
<br />

<ignore_js_op>

<img id="aimg_140823" aid="140823" src="static/image/common/none.gif" zoomfile="forum.php?mod=attachment&aid=MTQwODIzfGFlNzlmMWZifDE2MDk2MzAzNTF8NDczNDR8NzU5NTE0&noupdate=yes&nothumb=yes" file="forum.php?mod=attachment&aid=MTQwODIzfGFlNzlmMWZifDE2MDk2MzAzNTF8NDczNDR8NzU5NTE0&noupdate=yes" class="zoom" onclick="zoom(this, this.src, 0, 0, 0)" width="50" id="aimg_140823" inpost="1" onmouseover="showMenu({'ctrlid':this.id,'pos':'12'})" />

<div class="tip tip_4 aimg_tip" id="aimg_140823_menu" style="position: absolute; display: none" disautofocus="true">
<div class="xs0">
<p><strong>ico-firewall.png</strong> <em class="xg1">(1.21 KB, 下载次数: 0)</em></p>
<p>
<a href="forum.php?mod=attachment&amp;aid=MTQwODIzfGFlNzlmMWZifDE2MDk2MzAzNTF8NDczNDR8NzU5NTE0&amp;nothumb=yes" target="_blank">下载附件</a>

</p>

<p class="xg1 y">2020-10-28 18:35 上传</p>

</div>
<div class="tip_horn"></div>
</div>

</ignore_js_op>
系统防火墙<br />
官方&nbsp; &nbsp; &nbsp; &nbsp; <br />
提供系统防火墙(iptables/firewall/ufw)的可视化管理功能<br />


win的？直接进远程桌面啊

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9365553&amp;ptid=759514" target="_blank"><font color="#999999">hxuf 发表于 2020-10-28 18:36</font></a></font><br />
win的？直接进远程桌面啊</blockquote></div><br />
不，是CentOS

ssh进系统&nbsp;&nbsp;手动关防火墙吧<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

建议直接 dd

这边推荐重装系统呢

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9365577&amp;ptid=759514" target="_blank"><font color="#999999">liuyangge 发表于 2020-10-28 18:39</font></a></font><br />
ssh进系统&nbsp;&nbsp;手动关防火墙吧</blockquote></div><br />
我ssh小白啊，之前都玩WIN的。<br />
大概步骤能说下吗

ssh进去重启宝塔看看

centos <img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /> 有得玩了。<br />
开启firewall，又没开放端口，直接堵上了。。。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9365588&amp;ptid=759514" target="_blank"><font color="#999999">tkre 发表于 2020-10-28 18:41</font></a></font><br />
我ssh小白啊，之前都玩WIN的。<br />
大概步骤能说下吗</blockquote></div><br />
ssh连进系统，centos6就百度iptables关闭防火墙&nbsp;&nbsp;centos7就百度firewall关闭防火墙<br />
不过你可以先进ssh 输入 bt status 看下宝塔状态，可以输入bt命令重启下宝塔看看
