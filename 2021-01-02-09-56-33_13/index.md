# 求助一个200G的大文件如果拷贝到另外一台服务器


某服务器A有一个大文件，有200G，想拷贝到某服务器B，<br />
通过scp拷贝，拷贝了几十G后就速度变成0了，很奇怪，<br />
下面是我的命令：<br /><div class="blockcode"><div id="code_r22"><ol><li>scp -l 60000 -P 1234 -o IPQoS=throughput root@1.1.1.1:/home/image.tar.gz .<br /><li></ol></div><em onclick="copycode($('code_r22'));">复制代码</em></div><br />
不想弄rsync，配置感觉太复杂，<br />
老铁们们还有其他方案吗？<br />
求救...<br />
要后台可以执行的方法哦

resilio试试.go语言的.两个服务器都安装.然后a服务器选择那个文件夹进行分享然后就可以同步过去，而且是可以增量同步更新的

aria2c下载不行么？可以断点续传。<img src="static/image/smiley/default/tongue.gif" smilieid="7" border="0" alt="" />

rsync很简单的命令啊

使用 rclone<br />
上次有几千个文件 打包成 tar上传 GD盘<br />
然后在新机器上没看空间<br />
<br />
直接使用 rclone cat&nbsp;&nbsp;| tar 释放 搞下来

<img id="aimg_bGoFW" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/11/25/tPqDu1AFI2ipKSx.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9513926&amp;ptid=771136" target="_blank"><font color="#999999">guyuefeng 发表于 2020-11-25 11:19</font></a></font><br />
rsync很简单的命令啊</blockquote></div><div class="blockcode"><div id="code_x11"><ol><li>rsync -auvzP --bwlimit=6000 -e &quot;ssh -p1234&quot; root@1.1.1.1:/home/image.tar.gz .</ol></div><em onclick="copycode($('code_x11'));">复制代码</em></div><br />
我试试这个rsync

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9513935&amp;ptid=771136" target="_blank"><font color="#999999">sRGB 发表于 2020-11-25 11:20</font></a></font><br />
使用 rclone<br />
上次有几千个文件 打包成 tar上传 GD盘<br />
然后在新机器上没看空间</blockquote></div><br />
谢谢，我先试试rsync，不行的话我试试rclone

lftp<br />
多线程

一个文件用wget吧。
