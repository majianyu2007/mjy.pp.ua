# SYN FLOOD攻击和cc攻击具体有什么区别


SYN FLOOD攻击，攻击方式。这是一种使用TCP协议缺陷，发送大量的伪造的TCP连接请求，使得被攻击方cpu或内存资源耗尽，最终导致被攻击方无法提供正常的服务<br />
<br />
cc攻击，是攻击者控制某些主机不停地发大量数据包给对方服务器造成服务器资源耗尽，一直到宕机崩溃。CC主要是用来攻击页面的，每个人都有这样的体验：当一个网页访问的人数特别多的时候，打开网页就慢了，CC就是模拟多个用户(多少线程就是多少用户)不停地进行访问那些需要大量数据操作(就是需要大量CPU时间)的页面，造成服务器资源的浪费，CPU长时间处于100%，永远都有处理不完的连接直至就网络拥塞，正常的访问被中止。<br />
<br />
<br />
（1）SYN FLOOD攻击和cc攻击具体有什么区别？<br />
<br />
（2）syn flood攻击和cc攻击都是耗尽服务器的内存和CPU，哪么syn flood攻击能不能理解成是cc攻击的一种呢？<br />
<br />
（3）SYN FLOOD攻击又要怎么防，普通防火墙能防的住吗?<br />
<br />
<br />
<br />
求各位大佬解惑

一个是堵你大门，一个是占着茅坑不拉屎

<i class="pstatus"> 本帖最后由 蓝色梦想 于 2020-10-23 10:11 编辑 </i><br />
<br />
flood是把你的商店塞满人<br />
cc是把你的商店里面的工作人员和机器全都控制住<br />
结果基本一样，让你瘫痪<img id="aimg_s0c2Z" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339724&amp;ptid=757496" target="_blank"><font color="#999999">蓝色梦想 发表于 2020-10-23 10:09</font></a></font><br />
flood是堵门<br />
cc是堵人<br />
结果基本一样，让你瘫痪</blockquote></div><br />
防火墙可以防的住吗

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339734&amp;ptid=757496" target="_blank"><font color="#999999">小丶雨 发表于 2020-10-23 10:11</font></a></font><br />
防火墙可以防的住吗</blockquote></div><br />
要看对方的攻击力度<img id="aimg_J6c26" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

我觉得跟半连接队列有关系把

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339752&amp;ptid=757496" target="_blank"><font color="#999999">蓝色梦想 发表于 2020-10-23 10:12</font></a></font><br />
要看对方的攻击力度</blockquote></div><br />
懂了，只要攻击补偿过防火墙的上线就没问题了，谢谢大佬解惑<img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" />

黑洞防火墙可以挡一部分

区别有点，7楼

<br />
SYN FLOOD攻击&nbsp; &nbsp;在4层，用硬件防火墙，过滤掉就行了，<br />
cc&nbsp;&nbsp;在7层， 用软防找到特征防御
