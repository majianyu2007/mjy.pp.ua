# 各位求救啊，IPTABLES的！！！


有啥好的办法没，。。。<br />
<br />
打个比方，不允许用户访问google.com 并返回一个禁止访问的页面到他的浏览器。<br />
<br />
网站是用iptables直接DROP了的！

本机开个web服务器，专门显示那个禁止访问的页面，然后redirect过去。

<i class="pstatus"> 本帖最后由 diocat 于 2020-10-23 14:46 编辑 </i><br />
<br />
匹配后dnat到某台机的http端口上<br />
<br />
当然只dnat是不行的，还缺一个也是nat，自己写

DNS劫持更好操作一些

难搞，不知道怎么恢复你的问题

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9341191&amp;ptid=757601" target="_blank"><font color="#999999">diocat 发表于 2020-10-23 14:45</font></a></font><br />
匹配后dnat到某台机的http端口上<br />
<br />
当然只dnat是不行的，还缺一个也是nat，自己写 ...</blockquote></div><br />
iptables -t nat -A PREROUTING -d google.com -p tcp -m tcp --dport 80 -j DNAT --to-destination baidu.com<br />
<br />
访问google跳转baidu&nbsp;&nbsp;去

用iptables&nbsp;&nbsp;string模块，但是我只能做到丢弃数据包，没办法返回一个禁止访问的页面<br />
<br />
iptables -A OUTPUT -m string --string &quot;google.com&quot; --algo bm --to 65535 -j DROP

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9341236&amp;ptid=757601" target="_blank"><font color="#999999">forever8938 发表于 2020-10-23 14:55</font></a></font><br />
本机开个web服务器，专门显示那个禁止访问的页面，然后redirect过去。</blockquote></div><br />
<br />
要求：请求服务器A的80，由A转到服务器B<br />
环境：<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;A：iptables&nbsp; &nbsp;google.com<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;B：baidu.com<br />
<br />
在A上做下面设置<br />
iptables -t nat -A PREROUTING -d google.com -p tcp --dport 80 -j DNAT --to baidu.com:80<br />
iptables -t nat -A POSTROUTING -d baidu.com -p tcp --dport 80 -j SNAT --to google.com<br />
<br />
访问 google.com 就会显示baidu.com的web内容

做不到，你可能需要7层协议解析之后过滤才行，例如haproxy

<img id="aimg_j54m5" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://mjjzp.cf/2020/10/23/c4d31e12a982c.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
