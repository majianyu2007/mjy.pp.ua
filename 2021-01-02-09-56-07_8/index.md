# solusvm 开出的openvz小鸡不能解析域名


<i class="pstatus"> 本帖最后由 mrludan1994 于 2020-11-6 10:29 编辑 </i><br />
<br />
solusvm 开出的openvz小鸡不能解析域名，可以ping通外网IP，如何解决？

换DNS 肯定是DNS 坏了

dns 或者br0的问题

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403042&amp;ptid=762454" target="_blank"><font color="#999999">vzker 发表于 2020-11-4 18:52</font></a></font><br />
换DNS 肯定是DNS 坏了</blockquote></div><br />
感觉是小鸡没有自动分配到DNS服务器。不知道怎么解决。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403067&amp;ptid=762454" target="_blank"><font color="#999999">mrludan1994 发表于 2020-11-4 18:57</font></a></font><br />
感觉是小鸡没有自动分配到DNS服务器。不知道怎么解决。</blockquote></div><br />
手动改呀 windows我就不说了 linux一般是 /etc/resolv.conf
