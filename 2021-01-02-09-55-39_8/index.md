# 云厂商用自建的DNS是真的坑


<i class="pstatus"> 本帖最后由 问世间情为何物 于 2020-10-24 21:42 编辑 </i><br />
<br />
不管国内的还是国外的，稍微大点的厂商都喜欢自建DNS。<br />
自建完了一堆坑。<br />
<br />
比如已经遇到过的：<br />
限制请教次数，请求多了就封IP<br />
新解析生效时间超慢<br />
<br />
<br />
<br />
一天天的就知道女票，DNS有个JB好女票的？如果用114.114.114.114 8.8.8.8一点问题不会有，哪个收费了？厂家非得自己搞，搞完了又TM一堆坑。

不自建一个，又说连个dns都没有。<br />
付费又不愿意付费。白女票还挑三拣四。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347724&amp;ptid=758023" target="_blank"><font color="#999999">问世间情为何物 发表于 2020-10-24 21:27</font></a></font><br />
张嘴就知道女票，女票个几把啊，你见哪个公共DNS收费了？</blockquote></div><br />
不说清楚，谁知道你说的是公共dns。<br />
公共就是大家用的。<br />
搞的都被别人限制请求次数，涉嫌攻击dns了，还有理了。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347588&amp;ptid=758023" target="_blank"><font color="#999999">斜阳晚暮 发表于 2020-10-24 20:59</font></a></font><br />
不自建一个，又说连个dns都没有。<br />
付费又不愿意付费。白女票还挑三拣四。 ...</blockquote></div><br />
张嘴就知道女票，女票个几把啊，你见哪个公共DNS收费了？

不然怎么坑你买付费服务

选Google、Amazon、Microsoft这种体量的公司就基本不会出问题了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347588&amp;ptid=758023" target="_blank"><font color="#999999">斜阳晚暮 发表于 2020-10-24 20:59</font></a></font><br />
不自建一个，又说连个dns都没有。<br />
付费又不愿意付费。白女票还挑三拣四。 ...</blockquote></div><br />
在理

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347279&amp;ptid=758023" target="_blank"><font color="#999999">why? 发表于 2020-10-24 19:55</font></a></font><br />
不然怎么坑你买付费服务</blockquote></div><br />
<br />
公共DNS，国内114.114.114.114，国外8.8.8.8，啥问题都不会有，付个JB费。<br />
<br />
厂商非得自己搞，搞完又TM不稳定。

<i class="pstatus"> 本帖最后由 jqbaobao 于 2020-10-24 21:32 编辑 </i><br />
<br />
https://dns.google/dns-query<br />
tls://dns.google<br />
https://dns.cloudflare.com/dns-query<br />
tls://1.1.1.1<br />
https://dns.alidns.com/dns-query<br />
tls://dns.alidns.com<br />
https://doh.pub/dns-query<br />
https://dns.pub/dns-query<br />
tls://dns.pub<br />
<br />
<br />
所以说自建不是最好吗<br />
<br />
<img id="aimg_qdbgD" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://img14.360buyimg.com/ddimg/jfs/t1/145040/39/11848/130183/5f942cc3Eefbfdb3c/0c8802e1a885f2d8.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
<img id="aimg_kEJ2n" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="596" src="https://img14.360buyimg.com/ddimg/jfs/t1/139835/17/11970/61837/5f942cf7E04b678b1/2c9ec0556a34ab64.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" />

公共dns限制请求次数？？？

这个确实是个痛点，挺蛋疼的。<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />
