# 【更新】一键网络重装系统 - 魔改版（适用于Linux / Windows）


<i class="pstatus"> 本帖最后由 MeowLove 于 2020-9-21 15:34 编辑 </i><br />
<br />
<img id="aimg_sl1P1" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/09/15/DR1jkHBzJIpaT8c.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
<font size="5">简介</font><br />
<br />
<font size="4">这还要介绍？？懒得写了。</font><br />
<br />
<br />
<font size="5">魔改版本及开源地址</font><br />
<br />
<font size="4">最新版本：3.1.0（2020/09/15）<br />
<br />
官方发布：https://www.cxthhhhh.com/network-reinstall-system-modify<br />
<br />
Github：Network-Reinstall-System-Modify<br />
<br />
魔改版本：CXTHHHHH (via) 原始版本：MoeClub(Vicer)</font><br />
<br />
<br />
<font size="5">支持安装的系统</font><br />
<br />
<font size="4">Alpine Linux、Anarchy Linux、Arch Linux、Backbox、BlackArch Linux、Bluestar Linux、Bodhi Linux、CentOS、CoreOS、Debian、Deepin、Devuan、Elementary OS、Fedora、Feren OS、Flatcar Linux、FreeBSD、FreeDOS、Gentoo、IPFire、Kali Linux、KDE Neon、Kodachi、Linux Lite、Q4OS、Microsoft Windows、Mageia、Manjaro、Mint、MirOS、Nitrux、NixOS、OpenBSD、OpenSUSE、Oracle Linux、Parrot Security、Peppermint、Proxmox-VE、Pop OS、Red Hat Enterprise Linux、Regolith、RancherOS、Scientific Linux、Slackware、SparkyLinux、Tails、Tiny Core Linux、Ubuntu、Velt、Voyager、Zen Installer、Zorin OS、ALT Linux Rescue、Boot Repair CD、Breakin、CAINE、Clonezilla、DBAN、GParted、Grml、Memtest、Rescatux、Super Grub2 Disk、System Rescue CD、Ultimate Boot CD</font><br />
<br />
<br />
<font size="5">怎么用？</font><br />
<br />
<font size="4">复制粘贴2行命令，回车。合并后甚至一条命令足以。</font><br />
<br /><div class="blockcode"><div id="code_rFK"><ol><li>wget --no-check-certificate -qO ~/Network-Reinstall-System-Modify.sh 'https://www.cxthhhhh.com/CXT-Library/Network-Reinstall-System-Modify/Network-Reinstall-System-Modify.sh' &amp;&amp; chmod a+x ~/Network-Reinstall-System-Modify.sh &amp;&amp; bash ~/Network-Reinstall-System-Modify.sh -UI_Options</ol></div><em onclick="copycode($('code_rFK'));">复制代码</em></div><br />
<br />
<br />
<font size="5">这里主要写一下这次更新的说明吧</font><br />
<br />
<font size="4">新增 图形化安装选项<br />
新增 Ubuntu 20.04<br />
新增 前置自动部属<br />
新增 安全警示<br />
更新 裸机系统部署平台<br />
更新 CentOS 8/7</font><br />
<br />
<br />
<font size="5">最后</font><br />
<br />
<font size="4">感谢Vicer、云图、老司机、VShare、Wei He、salty、rc4md5，coy等，以及各位大佬就对了。大佬们牛逼！</font><br />
<br />
<br />
<font size="5">组**流</font><br />
<br />
<font size="4">https://t.me/me_share<br />
https://t.me/CXTHHHHH</font><br />
<br />
<font size="5">交流讨论（频道、组群、论坛）</font><br />
<br />
<font size="4">了解【联系我们（Contact-US）https://www.cxthhhhh.com/contact-us】页面获得更多信息</font><br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9173867&amp;ptid=744083" target="_blank"><font color="#999999">lkkle 发表于 2020-9-15 14:36</font></a></font><br />
# Install<br />
<br />
Auto Mode insatll&nbsp;&nbsp;[focal] [amd64]. </blockquote></div><br />
众所周知，发布页说明都懒得看。。<br />
给你框起来了，提供优质的解答服务。<br />
<br />
<img id="aimg_w43i9" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/09/15/CK1oqIwGUtkvygf.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9173666&amp;ptid=744083" target="_blank"><font color="#999999">便宜主机推荐 发表于 2020-9-15 14:02</font></a></font><br />
支持一下，大佬Nb，这就给小鸡安装一个PVE去</blockquote></div><br />
早就可以了，去年就可以。我之前在群里只说了简要的操作过程，然后大佬们自己折腾去了。<br />
群里有大佬早就开玩了。只是我一直没写博文介绍详细过程，要自己摸索。<br />
<br />
这周末撸一篇Pve安装出来。

<div class="quote"><blockquote><font color="#999999">Zynstream 发表于 2020-9-18 17:29</font><br />
<font color="#999999">想dd成centos7及以上的，甲骨文的别用，直接失联，VNC都就不回来。已经试过无数次了，无论原系统是oracle的 ...</font></blockquote></div><br />
裸机系统部署平台不能用吗？自己不会，还VNC都救不回来。笑死了。

<i class="pstatus"> 本帖最后由 llyang 于 2020-9-16 16:39 编辑 </i><br />
<br />
刚才在ruvds上面安装debain10报错<br />
现有OS ubuntu 18<br /><div class="blockcode"><div id="code_ePN"><ol><li># Install<br /><li><br /><li>Auto Mode insatll [Debian] [buster] [amd64]. <br /><li><br /><li>[Debian] [buster] [amd64] Downloading...<br /><li>Not found `ip command`, It will use `route command`.<br /><li>Error! Not configure network. <br /><li>---------------------------------------------------------------------------------------------------------------------<br /><li> Start Installation <br /><li> Start Installation <br /><li>---------------------------------------------------------------------------------------------------------------------<br /><li><br /><li></ol></div><em onclick="copycode($('code_ePN'));">复制代码</em></div><br />
<br />
<font color="Red">我单独运行下面命令是正常的<br />
</font><div class="blockcode"><div id="code_YnY"><ol><li>ip route show</ol></div><em onclick="copycode($('code_YnY'));">复制代码</em></div><br />
<br />
截取字段似乎出问题了，我得到的是下面结果，供你未来改进用<br /><div class="blockcode"><div id="code_dr8"><ol><li>default via 194.22.144.1 dev eth0 <br /><li>194.22.144.0/22 dev eth0 proto kernel scope link src 194.22.144.99</ol></div><em onclick="copycode($('code_dr8'));">复制代码</em></div><br />
上面IP地址非真实，格式正确<br />
<br />
ip addr<br /><div class="blockcode"><div id="code_JD1"><ol><li>1: lo: &lt;LOOPBACK,UP,LOWER_UP&gt; mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000<br /><li>&nbsp; &nbsp; link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00<br /><li>&nbsp; &nbsp; inet 127.0.0.1/8 scope host lo<br /><li>&nbsp; &nbsp;&nbsp; &nbsp; valid_lft forever preferred_lft forever<br /><li>&nbsp; &nbsp; inet6 ::1/128 scope host <br /><li>&nbsp; &nbsp;&nbsp; &nbsp; valid_lft forever preferred_lft forever<br /><li>2: eth0: &lt;BROADCAST,MULTICAST,UP,LOWER_UP&gt; mtu 1500 qdisc mq state UP group default qlen 1000<br /><li>&nbsp; &nbsp; link/ether 00:15:5d:0a:69:bb brd ff:ff:ff:ff:ff:ff<br /><li>&nbsp; &nbsp; inet 194.22.144.109/22 scope global eth0<br /><li>&nbsp; &nbsp;&nbsp; &nbsp; valid_lft forever preferred_lft forever<br /><li>&nbsp; &nbsp; inet6 fe80::215:5dff:fe0a:60bb/64 scope link <br /><li>&nbsp; &nbsp;&nbsp; &nbsp; valid_lft forever preferred_lft forever<br /><li></ol></div><em onclick="copycode($('code_JD1'));">复制代码</em></div><br />
<br />
<br />
echo &quot;$GATE&quot; #194.22.144.1 正常<br />
echo &quot;$MASK&quot; #返回空值<br />
echo &quot;$IPv4&quot; #返回空值<br />
<br />
<br />
真实值是 netmask 255.255.252.0<br />
<br />
手工输入安装。。。。石头盘，估计需要1小时时间。<br />
<br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9173898&amp;ptid=744083" target="_blank"><font color="#999999">MeowLove 发表于 2020-9-15 14:42</font></a></font><br />
众所周知，发布页说明都懒得看。。<br />
给你框起来了，提供优质的解答服务。</blockquote></div><br />
已经测试过了，在甲骨文centos7下该脚本运行安装后无效，<br />
有一点不错，其它脚本会让甲骨文小鸡失联，楼主的脚本运行后会重启小鸡，但是安装不了，还是默认系统，因为SSH还能连上

大佬，这个能不能用于甲骨文的鸡？ 大概是uefi的

甲骨文可以DD吗

这玩意物理机行不行 <br />
情况是这样<br />
<br />
比如说 物理机有 网口 1 -4&nbsp;&nbsp;<br />
即 em1 em2 em3 em4 <br />
如果我网线配置再em4上是公网&nbsp; &nbsp;em1 是 dhcp的内网 <br />
这东西安装完了结果是不是失联了?

谢谢分享，非常需要！<br />
<br />
大佬厉害！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

来了，支持一下，虽然用老咖的比较多

支持下<br />
求优化cc小鸡安装<br />


前排支持大佬<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img id="aimg_WdL3u" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

大佬又来更新了，收藏下，感谢！

这是干嘛的那？？

支持一下，大佬Nb，这就给小鸡安装一个PVE去<img id="aimg_FTXOU" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

支持支持,mark一下<img src="static/image/smiley/yct/019.gif" smilieid="49" border="0" alt="" />

大佬牛逼<img src="static/image/smiley/yct/017.gif" smilieid="40" border="0" alt="" />
