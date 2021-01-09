# 2台服务器，一台中转，中转只能用IP吗？


<i class="pstatus"> 本帖最后由 gzaer 于 2020-11-1 15:56 编辑 </i><br />
<br />
一台国外服务器A，nginx+web+tls+域名<br />
一台国内服务器B，用Socat进行转发，客户端填写的就是B的服务器IP<br />
<br />
我想把B套上CF，那客户端填的就是域名了，这个该怎么操作，应该在B服务器上安装个ngix吗？<br />
<br />
国内（IP地址）→国外(CF域名)，开启了中转，客户端应该填的就是国内的IP地址吧，我就是想如何把国内的IP换成域名的形式，这样客户端填的就是域名了<br />
<br />
也就是国内（域名）→国外(CF域名)

我不太懂，知识盲区了 楼下知道吗 

B套CF? 封包從國內→國外(CF)→國內(B)→國外(A)，出入境4次，延遲沒問題嗎？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9385079&amp;ptid=760950" target="_blank"><font color="#999999">s920361 发表于 2020-11-1 15:35</font></a></font><br />
B套CF? 封包從國內→國外(CF)→國內(B)→國外(A)，出入境4次，延遲沒問題嗎？</blockquote></div><br />
那开机场的人是怎么搞的？不可能用户填的都是中转机器的IP吧

iptables有直接转发域名的脚本！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9385118&amp;ptid=760950" target="_blank"><font color="#999999">llmwxt 发表于 2020-11-1 15:46</font></a></font><br />
iptables有直接转发域名的脚本！</blockquote></div><br />
不是转发域名，是指中转机配置域名，然后客户端上填的是域名

<i class="pstatus"> 本帖最后由 VULLUV 于 2020-11-1 16:13 编辑 </i><br />
<br />
socat保持端口不变的话，域名直接解析到中转机IP即可<br />
不过你这又套CF又要中转的操作就很迷惑

我文化水平低<br />
这个不是直接域名解析到中转机就可以了吗？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9385243&amp;ptid=760950" target="_blank"><font color="#999999">damoo 发表于 2020-11-1 16:23</font></a></font><br />
我文化水平低<br />
这个不是直接域名解析到中转机就可以了吗？</blockquote></div><br />
解析的话 需要nginx绑定吗？ 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9385210&amp;ptid=760950" target="_blank"><font color="#999999">VULLUV 发表于 2020-11-1 16:12</font></a></font><br />
socat保持端口不变的话，域名直接解析到中转机IP即可<br />
不过你这又套CF又要中转的操作就很迷惑 ...</blockquote></div><br />
我懂了，谢谢
