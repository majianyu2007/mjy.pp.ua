# 求大神教：SOLUSVM开KVM的nat小鸡，小鸡不能访问外网。


求大神教：SOLUSVM开KVM的nat小鸡，小鸡不能访问外网。<br />
<br />
<br />
是在局域网测试的，母鸡可以访问外网，已经官方教程说的搭建网桥。<br />
<br />
<br />
分配给小鸡的IP是10.0.1.199&nbsp; &nbsp;母鸡设置的10.0.1.1&nbsp; &nbsp;母鸡外网接的家里路由器网关 192.168.100.10<br />
<br />
目前情况：小鸡可以ping通母鸡的10.0.1.1&nbsp;&nbsp;母鸡也可以ping通小鸡的10.0.1.199<br />
<br />
但是小鸡无法访问外网，也访问不了家里网关192.168.100.10<br />
<br />
<br />
-------------------------------母鸡相关配置如下---------------------------------------<br />
<br />
/etc/sysconfig/network-scripts&nbsp;&nbsp;下的配置文件<br />
<br />
<img id="aimg_X5zoG" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://pic.rmb.bdstatic.com/bjh/32e30c9551635f4c050d68730c60dc27.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
<br />
<img id="aimg_sS858" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://pic.rmb.bdstatic.com/bjh/a32bf3b9b7211f287597d740870ea8a1.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<img id="aimg_nW87o" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://pic.rmb.bdstatic.com/bjh/0e3c289aa367f85fb470733a27f3b739.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<img id="aimg_Jcx7Y" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://pic.rmb.bdstatic.com/bjh/2843970229756f6f2916d59d091161e4.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
网桥情况：<br />
<img id="aimg_A7fC1" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://pic.rmb.bdstatic.com/bjh/adce0ae35111f6d9fdd6ef27b7d51499.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
-------------------------------小鸡相关信息---------------------------------------<br />
<br />
不能访问外网<br />
<img id="aimg_p50Dc" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://pic.rmb.bdstatic.com/bjh/c1f55a8fc53656bc724bd72ce71ee2e7.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
可以通母鸡<br />
<img id="aimg_I44N6" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://pic.rmb.bdstatic.com/bjh/028a9221cc20e5519bb2c1292fba8359.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />


我不懂，楼下技术大佬来。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9410646&amp;ptid=763133" target="_blank"><font color="#999999">yanaxiao 发表于 2020-11-6 10:23</font></a></font><br />
我不懂，楼下技术大佬来。</blockquote></div><br />
你楼下来的是小白，技术一点不懂！<br />
<br />
<img src="static/image/smiley/default/funk.gif" smilieid="29" border="0" alt="" />

求大神教

不懂 帮顶 等大佬<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

求懂的大佬赐教。zsbd

10块吃个包子给你一条命令<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

你需要设置iptables，具体的百度吧

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9410733&amp;ptid=763133" target="_blank"><font color="#999999">mrludan1994 发表于 2020-11-6 10:36</font></a></font><br />
求大神教</blockquote></div><br />
<a href="https://www.hostloc.com/home.php?mod=space&amp;uid=46341" target="_blank">@dxt</a>&nbsp;&nbsp;来接客了，10元一位<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />
