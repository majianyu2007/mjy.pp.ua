# Buyvm家的小鸡绑定IPv6地址


<i class="pstatus"> 本帖最后由 edear 于 2020-10-18 02:10 编辑 </i><br />
<br />
不想找客服弄，自己搞定了, 就两步:<br />
<br />
第一步、编辑netplan配置文件<br />
$ sudo vi /etc/netplan/01-netcfg.yaml<br /><div class="blockcode"><div id="code_ZCI"><ol><li><br /><li># This file describes the network interfaces available on your system<br /><li># For more information, see netplan(5).<br /><li><br /><li>network:<br /><li>&nbsp;&nbsp;version: 2<br /><li>&nbsp;&nbsp;renderer: networkd<br /><li>&nbsp;&nbsp;ethernets:<br /><li>&nbsp; &nbsp; eth0:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;dhcp4: yes<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;dhcp6: no<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;addresses:<br /><li>&nbsp; &nbsp;&nbsp;&nbsp;- 2605:6400:0020:001e:0651:XXXX:XXXX:XXXX/48<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;gateway6: 2605:6400:20::1<br /><li></ol></div><em onclick="copycode($('code_ZCI'));">复制代码</em></div><br />
<br />
第二步、让netplan配置生效：<br />
$ sudo netplan apply<br />
<br />
测试结果<br />
<img id="aimg_zc9qE" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://preview.cloud.189.cn/image/imageAction?param=F41D99E95CAB7335D2DB3EECD56DBEA3DA1633F46468144EC4FA0E33E69BEB84C60D1FE0DF1607192B0FA5447261AAFCAB4B3B658E911E42A2868EB7B96E0B4902372FD14A71B35C9AA48474FACEB87D3769036E8FC3D7781D6D6219" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />


编辑：/etc/network/interfaces 添加ipv6 配置就可以了。<br />
先在面板里添加ipv6 ，然后查看下ip地址和gateway 网关。<br /><div class="blockcode"><div id="code_x9U"><ol><li>iface eth0 inet6 static<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;address 2605:6400:0020:163f:a9f8:39ba:549d:165a<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;netmask 48<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;gateway 2605:6400:0020:0000:0000:0000:0000:0001</ol></div><em onclick="copycode($('code_x9U'));">复制代码</em></div><br />
保存，重启。<br />
<br />
网上找的教程。你试试。

搜ubuntu18以上的教程，改yaml文件

顺便说一句，debian的v6我从来没成功配置过。。

算了，让客服去弄了，回头给大家汇报一下

铜球，我的是c7的<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9315792&amp;ptid=755505" target="_blank"><font color="#999999">小俊哟 发表于 2020-10-18 00:44</font></a></font><br />
铜球，我的是c7的</blockquote></div><br />
我在顶楼贴出答案了

ipv6地址在哪里搞鸭，楼主<img src="static/image/smiley/default/biggrin.gif" smilieid="3" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9316234&amp;ptid=755505" target="_blank"><font color="#999999">小俊哟 发表于 2020-10-18 09:29</font></a></font><br />
ipv6地址在哪里搞鸭，楼主</blockquote></div><br />
自带的吧

<div class="quote"><blockquote><font color="#999999">小俊哟 发表于 2020-10-18 09:29</font><br />
<font color="#999999">ipv6地址在哪里搞鸭，楼主</font></blockquote></div><br />
他家的v6地址是送的，自己在面板上添加，要多少有多少
