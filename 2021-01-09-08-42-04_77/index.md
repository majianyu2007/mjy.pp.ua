# 局域网文件共享方案


用途：用于内网各部门文件共享<br />
要求：各部门共享文件分开用户名密码，本部门不能访问其他部门信息<br />
现在方案：现在在用win 2016 server 只是开了文件夹共享，不同部门不同ID权限和文件夹<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;但是发现一个问题，A部门添加网络磁盘后，不能再添加B部门的网络磁盘，因为A部门的密码没有B部门共享文件夹的权限<br />
<br />
<br />
<strong><font size="5">求靠谱方案</font></strong>

学习windows的用户和组，小学生，

你这样还是用软件解决吧 比如网盘软件 设置好权限就行了 

好复杂，我帮顶吧！<br />
<br />
<img src="static/image/smiley/default/sad.gif" smilieid="2" border="0" alt="" /><img src="static/image/smiley/default/sad.gif" smilieid="2" border="0" alt="" /><img src="static/image/smiley/default/sad.gif" smilieid="2" border="0" alt="" />

ftp设置不同用户不同根目录？<img id="aimg_qTtgA" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375808&amp;ptid=760293" target="_blank"><font color="#999999">周润发 发表于 2020-10-30 16:21</font></a></font><br />
你这样还是用软件解决吧 比如网盘软件 设置好权限就行了</blockquote></div><br />
unraid,群晖到可道云，这些都能解决，但是我想找最简单的方法，仅仅是文件共享，没必要用到群晖这类东西

你都分开了，还加别的部门的干啥<br />
干脆改linux<br />
分多个网盘程序部署了不就行了<br />
一个部门一个端口

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375818&amp;ptid=760293" target="_blank"><font color="#999999">sqliuchang 发表于 2020-10-30 16:22</font></a></font><br />
ftp设置不同用户不同根目录？</blockquote></div><br />
现在是共享设不同用户不同根目录文件夹，

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375830&amp;ptid=760293" target="_blank"><font color="#999999">zgs 发表于 2020-10-30 16:24</font></a></font><br />
你都分开了，还加别的部门的干啥<br />
干脆改linux<br />
分多个网盘程序部署了不就行了</blockquote></div><br />
举个栗子？比如？

还是群晖比较靠谱
