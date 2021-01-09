# dd的debian, tab 不能补全 docker 的命令


dd的debian, tab 不能补全 docker 的命令<br />
仅仅docke命令不能补全当然也许我用的命令比较少，系统基本命令都能补全。docker 确定是不能补全<br />
这是为何？

不能补全命令，管 debian 什么事，你不问下你 shell 吗<img id="aimg_UL1Jv" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="blockcode"><div id="code_jRR"><ol><li>sudo apt install -y bash-completion</ol></div><em onclick="copycode($('code_jRR'));">复制代码</em></div><br />
<br />
试试安装自动补全，不过我记得Debian系是自带的，CentOS才需要自己装。

用的是这个<br />
https ://www.mcxiaofan.cn/sh/dd.sh

那就用Ubuntu吧

/etc/profile

如果你指的是docker后面的ps -d的参数啥的话。确实补全不了吧。。 输入dock 按tab倒是能补全出docker

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9360142&amp;ptid=758963" target="_blank"><font color="#999999">nisekoi 发表于 2020-10-27 17:24</font></a></font><br />
如果你指的是docker后面的ps -d的参数啥的话。确实补全不了吧。。 输入dock 按tab倒是能补全出docker ...</blockquote></div><br />
vps自带的系统,docker 后的命令都能补全，dd的，docker后的命令都不能补全。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9360082&amp;ptid=758963" target="_blank"><font color="#999999">吴佳炜 发表于 2020-10-27 17:06</font></a></font><br />
/etc/profile</blockquote></div><br />
刚刚对比了，dd的与非dd的，debian。里面的/etc/profile 内容完全相同
