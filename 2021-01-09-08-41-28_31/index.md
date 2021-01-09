# HZ杜甫安装win的正确姿势？


用的萌咖大佬的脚本 DD后失联了<br /><div class="blockcode"><div id="code_Afm"><ol><li>wget --no-check-certificate -qO InstallNET.sh 'https://moeclub.org/attachment/LinuxShell/InstallNET.sh' &amp;&amp; bash InstallNET.sh -dd 'http://d.nat.ee/win10/win10-ltsc-x64-cn.vhd.gz'</ol></div><em onclick="copycode($('code_Afm'));">复制代码</em></div>

还有不推荐DD，<br />
直接点击support 申请KVM，Comment:里面填入：<br />
resinstall OS,<br />
Please put the following ISO file into the U disk and insert it into my server. Thank you<br />
<br />
https://windows.iso.st/从这里面随便选一个直链放到最后，静静等待10分钟就可以了

第一步：安装Centos7或者8进入执行下面命令<br />
bash &lt;(curl -s -S -L https://file.iso.st/CentosNetReInstall.sh)<br />
选择&nbsp;&nbsp;自定义ISO选项，输入ISO直链，或者 PE模式<br />
回车回车会关机<br />
第二步：后台开启 ，如图<br />
<img id="aimg_Waq3V" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/26/ElBIXofKMbvUpLc.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
第三步：网页登陆VKVM（NOVNC），然后按网页的C+A+D<br />
开机界面上下选择 startFromISO 回车，就可以进入ISO或者PE安装系统啦<br />
全程自己操作无后门 

试试论坛大佬的魔改版！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font color="#999999">llmwxt 发表于 2020-10-26 13:44</font><br />
<font color="#999999">试试论坛大佬的魔改版！</font></blockquote></div><br />
哪里搞

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353858&amp;ptid=758581" target="_blank"><font color="#999999">evils 发表于 2020-10-26 13:46</font></a></font><br />
哪里搞</blockquote></div><br />
搜索一下：魔改版<br />
<br />
就能看到帖子了！

你直接DD就好啦，不用脚本重装

<div class="quote"><blockquote><font color="#999999">llmwxt 发表于 2020-10-26 13:50</font><br />
<font color="#999999">搜索一下：魔改版<br />
<br />
就能看到帖子了！</font></blockquote></div><br />
找到了

<div class="quote"><blockquote><font color="#999999">ABCHINA 发表于 2020-10-26 13:59</font><br />
<font color="#999999">第一步：安装Centos7或者8进入执行下面命令<br />
bash</font></blockquote></div><br />
刚重装了ubuntu

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353940&amp;ptid=758581" target="_blank"><font color="#999999">evils 发表于 2020-10-26 14:01</font></a></font><br />
刚重装了ubuntu</blockquote></div><br />
兼容ubuntu和debian，但不一定保证成功，只在最新版本的debian和ubuntu做过实现
