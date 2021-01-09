# 【更新】一键网络重装系统 - 魔改版（适用于Linux / Windows）


如果是磁盘超过2TB<br />
使用网络重装,又没得IPMI之类的<br />
安装完后,磁盘是怎样的呢?

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354701&amp;ptid=744083" target="_blank"><font color="#999999">pony 发表于 2020-10-26 16:28</font></a></font><br />
如果是磁盘超过2TB<br />
使用网络重装,又没得IPMI之类的<br />
安装完后,磁盘是怎样的呢? ...</blockquote></div><br />
取决于使用的DD镜像的硬盘格式。<br />
<br />
DD脚本中最核心的一条命令是：<br /><div class="blockcode"><div id="code_fZq"><ol><li>wget -qO- '$DDURL' |gunzip -dc |/bin/dd of=\$(list-devices disk |head -n1)</ol></div><em onclick="copycode($('code_fZq'));">复制代码</em></div><br />
<br />
如果dd镜像的硬盘格式是MBR，DD之后vps硬盘的分区表格式MBR

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355038&amp;ptid=744083" target="_blank"><font color="#999999">proc 发表于 2020-10-26 17:26</font></a></font><br />
取决于使用的DD镜像的硬盘格式。<br />
<br />
DD脚本中最核心的一条命令是：</blockquote></div><br />
哦哦<br />
那么他这个...是支持大硬盘的,对吗?<br />
做RAID-0,几十个T...

# Check Dependence<br />
<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;iconv<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;wget<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;awk<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;grep<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;sed<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;cut<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;cat<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;cpio<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;gzip<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;find<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;dirname<br />
[ok]&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;basename<br />
Error! <br />
Not Found grub.<br />
---------------------------------------------------------------------------------------------------------------------<br />
 Start Installation <br />
 Start Installation <br />
<br />
请问下这是什么错误

收藏了帮顶帮顶<br />
大佬

大佬你这博客终于能打开了<img id="aimg_V0N7G" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
