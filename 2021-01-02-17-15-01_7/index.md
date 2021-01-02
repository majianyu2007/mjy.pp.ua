# dd win win7 win8.1 win10 x64 甲骨文 直连分享


<i class="pstatus"> 本帖最后由 nat.ee 于 2020-9-22 18:04 编辑 </i><br />
<br />
VPS要求：<br />
系统：Debian7 或 Ubuntu12 以上<br />
仅支持KVM和XEN架构<br />
<br />
步骤1：安装运行库<br /><div class="blockcode"><div id="code_IBU"><ol><li>apt-get update<br /><li>apt-get install -y xz-utils openssl gawk file</ol></div><em onclick="copycode($('code_IBU'));">复制代码</em></div><br />
<br />
步骤2：一键安装<br />
<br />
(甲骨文专属) Windows 7 sp1 企业版 64位 精简版<br />
用户名：Administrator 密码：<a href="http://www.nat.ee" target="_blank">www.nat.ee</a> 系统最低要求：CPU：1核 内存：512M 硬盘：5G<br /><div class="blockcode"><div id="code_yi6"><ol><li>wget --no-check-certificate -qO InstallNET.sh 'http://d.nat.ee/sh/InstallNET.sh' &amp;&amp; bash InstallNET.sh -dd 'http://d.nat.ee/oracle/Uefi-gpt-Win7-Ent.gz'</ol></div><em onclick="copycode($('code_yi6'));">复制代码</em></div><br />
<br />
Windows 7 sp1 旗舰版 64位 精简版<br />
用户名：Administrator 密码：nat.ee 系统最低要求：CPU：1核 内存：512M 硬盘：5G<br /><div class="blockcode"><div id="code_zY9"><ol><li>wget --no-check-certificate -qO InstallNET.sh 'http://d.nat.ee/sh/InstallNET.sh' &amp;&amp; bash InstallNET.sh -dd 'http://d.nat.ee/win7/win7-ult-sp1-x64-cn.vhd.gz'</ol></div><em onclick="copycode($('code_zY9'));">复制代码</em></div><br />
<br />
Windows 8.1 专业版 64位 精简版<br />
用户名：Administrator 密码：nat.ee 系统最低要求：CPU：1核 内存：768M 硬盘：8G<br /><div class="blockcode"><div id="code_lE6"><ol><li>wget --no-check-certificate -qO InstallNET.sh 'http://d.nat.ee/sh/InstallNET.sh' &amp;&amp; bash InstallNET.sh -dd 'http://d.nat.ee/win8.1/win8.1-pro-x64-cn.vhd.gz'</ol></div><em onclick="copycode($('code_lE6'));">复制代码</em></div><br />
<br />
Windows 10 LTSC 企业版 64位 精简版<br />
用户名：Administrator 密码：nat.ee 系统最低要求：CPU：1核 内存：1G 硬盘：10G<br /><div class="blockcode"><div id="code_gN5"><ol><li>wget --no-check-certificate -qO InstallNET.sh 'http://d.nat.ee/sh/InstallNET.sh' &amp;&amp; bash InstallNET.sh -dd 'http://d.nat.ee/win10/win10-ltsc-x64-cn.vhd.gz'</ol></div><em onclick="copycode($('code_gN5'));">复制代码</em></div><br />
<br />
镜像站 提供 ISO，给那些家里挂虚拟机或者服务器商家支持挂载ISO镜像的人<br />
<a href="http://d.nat.ee" target="_blank">d.nat.ee</a><br />
<br />
特别注意，甲骨文和 win8.1镜像 支持kms 激活，需自行激活！<br />
甲骨文我以前制作了两个版本，一个是旗舰版，一个是最后更新制作的企业版，由于旗舰版激活困难，所以我之后制作了企业版支持kms激活，解决激活困难问题。<br />
<br />
没写甲骨文的，不支持甲骨文！<br />
<br />
更多详细信息，请访问镜像站，查看相应文件夹，有附带图片和制作说明内容，所有镜像均保留 net环境 iis nfs，等等。<br />
<br />
一键脚本 由 Vicer&amp;制作<br />
网站：MoeClub.org<br />
<br />
系统镜像 由 荣耀&amp;制作<br />
网站：nat.ee<br />
TG群：<a href="https://t.me/nat_ee" target="_blank">https://t.me/nat_ee</a>

为毛我之前DD就被封了号，现在没事了？

甲骨文被这么搞下去迟早药丸

有没有直连centos6的？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9207175&amp;ptid=746834" target="_blank"><font color="#999999">微笑着吃饭 发表于 2020-9-22 15:25</font></a></font><br />
甲骨文被这么搞下去迟早药丸</blockquote></div><br />
我的镜像站，没有放在甲骨文！并且我自己DD甲骨文win已经使用大半年，均正常，占用系统资源并不是99%加。

支持老司机

不放个MD5

前排支持 <img src="static/image/smiley/yct/011.gif" smilieid="33" border="0" alt="" />

<div class="quote"><blockquote><font color="#999999">小鱼 发表于 2020-9-22 15:41</font><br />
<font color="#999999">这么搞甲骨文，吃枣药丸</font></blockquote></div><br />
年初就分享了甲骨文win镜像，懂得都玩上了，现在才说药丸。<br />


前排支持~~~~~<img id="aimg_GBxFN" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
