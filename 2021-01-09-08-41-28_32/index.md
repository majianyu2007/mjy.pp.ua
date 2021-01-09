# HZ杜甫安装win的正确姿势？


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353949&amp;ptid=758581" target="_blank"><font color="#999999">ABCHINA 发表于 2020-10-26 14:03</font></a></font><br />
兼容ubuntu和debian，但不一定保证成功，只在最新版本的debian和ubuntu做过实现 ...</blockquote></div><br />
那我试下&nbsp;&nbsp;正好Ubuntu20

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353949&amp;ptid=758581" target="_blank"><font color="#999999">ABCHINA 发表于 2020-10-26 14:03</font></a></font><br />
兼容ubuntu和debian，但不一定保证成功，只在最新版本的debian和ubuntu做过实现 ...</blockquote></div><br />
启动救援后给的地址无法访问

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354099&amp;ptid=758581" target="_blank"><font color="#999999">evils 发表于 2020-10-26 14:35</font></a></font><br />
启动救援后给的地址无法访问</blockquote></div><br />
启动以后得从面板重启一下机器

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353930&amp;ptid=758581" target="_blank"><font color="#999999">ABCHINA 发表于 2020-10-26 13:59</font></a></font><br />
第一步：安装Centos7或者8进入执行下面命令<br />
bash</blockquote></div><br />
并没有出现从ISO启动...

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354164&amp;ptid=758581" target="_blank"><font color="#999999">evils 发表于 2020-10-26 14:49</font></a></font><br />
并没有出现从ISO启动...</blockquote></div><br />
是个英文，应该是最后一个，你的/boot分区可用空间得&gt;iso大小<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" />&nbsp;&nbsp;一般默认500M，pe刚刚好，我忘记说了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354178&amp;ptid=758581" target="_blank"><font color="#999999">ABCHINA 发表于 2020-10-26 14:52</font></a></font><br />
是个英文，应该是最后一个，你的/boot分区可用空间得&gt;iso大小&nbsp;&nbsp;一般默认500M，pe刚刚好，我忘记说 ...</blockquote></div><br />
那要怎么设置 boot 大小

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354191&amp;ptid=758581" target="_blank"><font color="#999999">evils 发表于 2020-10-26 14:54</font></a></font><br />
那要怎么设置 boot 大小</blockquote></div><br />
/boot是安装系统时候的初始分区。。<br />
比如HZ 救援模式安装系统installimage&nbsp; &nbsp; F10修改大小。找到/boot那一行直接用#注释掉。/boot就到/分区了，和/共享，这样一般是没问题的

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354191&amp;ptid=758581" target="_blank"><font color="#999999">evils 发表于 2020-10-26 14:54</font></a></font><br />
那要怎么设置 boot 大小</blockquote></div><br />
<br />
当然你可以用PE进去，我的PE支持联网（虚拟机驱动有 ），HZ应该可以的，不知道有没有网卡驱动。。。不过VKVM是以虚拟机模式启动的，应该可以<br />
<br />
不想折腾，就按照我的上面说的，申请KVM安装windows。直接给你挂在好ISO并且会给你引导到安装界面的

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354221&amp;ptid=758581" target="_blank"><font color="#999999">ABCHINA 发表于 2020-10-26 14:59</font></a></font><br />
当然你可以用PE进去，我的PE支持联网（虚拟机驱动有 ），HZ应该可以的，不知道有没有网卡驱动。。。不过V ...</blockquote></div><br />
<img id="aimg_I2lPD" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/26/DpuJzFf71Yi86Ua.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /> 你这脚本不行啊 c8
