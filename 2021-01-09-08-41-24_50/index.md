# 使用frp内网穿透，个人宽带不使用80,443等端口建站可以么


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9350485&amp;ptid=757616" target="_blank"><font color="#999999">chensbo 发表于 2020-10-25 17:12</font></a></font><br />
那干嘛不直接建在小鸡上</blockquote></div><br />
使用很多免费的frp服务，即使付费frp服务也非常的便宜。自己的小主机性能比小鸡强太多了。4核8G，配合frp服务10M带宽，这个配置非常强。

非标端口你跑啥都没人鸟你

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351656&amp;ptid=757616" target="_blank"><font color="#999999">lxyer 发表于 2020-10-25 22:41</font></a></font><br />
使用很多免费的frp服务，即使付费frp服务也非常的便宜。自己的小主机性能比小鸡强太多了。4核8G，配合frp ...</blockquote></div><br />
延迟太大还不如直接用小鸡了，除非只是个人访问或者对数据安全有要求。<br />


<div class="quote"><blockquote><font color="#999999">tsubasa 发表于 2020-10-25 20:56</font><br />
<font color="#999999">没有任何问题，你限制得只允许服务器访问，肯定是可以的。<br />
但是如果你过了SDN之类的设备，等于是无用……会 ...</font></blockquote></div><br />
frp走的不是web协议，走的是特殊的tcp或者udp协议

<div class="quote"><blockquote><font color="#999999">dragonfsky 发表于 2020-10-23 15:26</font><br />
<font color="#999999">可以吧 这样运营商也发现不了 我感觉最好的方法就是找个高位端口 然后弄个小鸡反向代理 再弄个只允许小鸡ip ...</font></blockquote></div><br />
那么不通过frp，有ipv4公网，是不是也可以反代下，只允许反代访问就行？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9352180&amp;ptid=757616" target="_blank"><font color="#999999">madebi 发表于 2020-10-26 05:43</font></a></font><br />
那么不通过frp，有ipv4公网，是不是也可以反代下，只允许反代访问就行？</blockquote></div><br />
有公网ip挺好的
