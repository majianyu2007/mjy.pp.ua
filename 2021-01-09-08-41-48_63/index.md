# IPV6网址升级改造有人接触过吗？


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9340036&amp;ptid=757469" target="_blank"><font color="#999999">shelizi1 发表于 2020-10-23 10:49</font></a></font><br />
大的机房换了，小的和老的就不好靠，运营商的流程慢的很，而且本身也有业务切换，运维技术反馈也慢。 ...</blockquote></div><br />
<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" />运营商硬件早支持了，底层是运营商的大问题。。。除非你接触的运营商的小的老的机房

腾讯云和阿里云都有ipv6了呀，直接申请开通ipv6，但是流量是分开计费的，也就是v4和v6都要收流量费，如果不想用这种方法，也可以开一个负载均衡，把机器用ipv6来负载，这样也具备ipv6了。<br />
如果是在运营商那自建服务器就更简单了，专线的话，告诉服务经理把v6打开，光纤拨号的话，在光猫上开ipv4/ipv6双栈打开，这样获取的就自动有/56的ipv6了。但是一定要桥接，一定要桥接，一定要桥接。不然ipv6入站数据自动丢

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339478&amp;ptid=757469" target="_blank"><font color="#999999">ABCHINA 发表于 2020-10-23 09:34</font></a></font><br />
IPV6延迟真的高。国内凑活一两百。。。只要一出国，延迟立马400往上</blockquote></div><br />
三家之间都是50以内呀，什么一两百，

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339487&amp;ptid=757469" target="_blank"><font color="#999999">shelizi1 发表于 2020-10-23 09:35</font></a></font><br />
小网站不需要，只有哪些被政策要求到的才会去做。主要是认证</blockquote></div><br />
就是骗这些地方的钱 哈哈哈<img id="aimg_Z0oX7" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

ipv6应该还是不成熟阶段,要真正能用可能还得好长一段时间<br />
<br />
现在好多app上面显示&nbsp;&nbsp;可以通过ipv6网络使用,完全就是骗人的<br />
纯ipv6网络下面根本不能使用<img id="aimg_gB7Zd" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9340300&amp;ptid=757469" target="_blank"><font color="#999999">jiangyang123 发表于 2020-10-23 11:51</font></a></font><br />
就是骗这些地方的钱 哈哈哈</blockquote></div><br />
上面有政策，不过也确实是能IPV6访问了。

用了好几年了，pt离不开。
