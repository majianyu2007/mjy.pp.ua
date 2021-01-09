# IPV6网址升级改造有人接触过吗？


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339471&amp;ptid=757469" target="_blank"><font color="#999999">dbug 发表于 2020-10-23 09:33</font></a></font><br />
都是些木有技术实力的被忽悠钱</blockquote></div><br />
小网站不需要，只有哪些被政策要求到的才会去做。主要是认证

关键是ipv6不能直接访问v4 网络

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339478&amp;ptid=757469" target="_blank"><font color="#999999">ABCHINA 发表于 2020-10-23 09:34</font></a></font><br />
IPV6延迟真的高。国内凑活一两百。。。只要一出国，延迟立马400往上</blockquote></div><br />
一般人也不访问IPV6吧，有什么用途吗？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339530&amp;ptid=757469" target="_blank"><font color="#999999">doctore 发表于 2020-10-23 09:41</font></a></font><br />
关键是ipv6不能直接访问v4 网络</blockquote></div><br />
对，所以需要把V4的网站改造成支持IPV6 V4双栈访问。不然现在全面把V4设备换成V6的成本太大了。<br />
<br />
先改造成双栈访问过渡。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339532&amp;ptid=757469" target="_blank"><font color="#999999">shelizi1 发表于 2020-10-23 09:42</font></a></font><br />
一般人也不访问IPV6吧，有什么用途吗？</blockquote></div><br />
<br />
windows10如果有IPV6的话，浏览器什么的都会默认走IPV6出口（如果服务提供的话），很慢，真的垃圾。设置IPV4优先，还得去微软官网下载补丁重启才行。<br />
不然打开一些国外网站你打开半天都打不开的。除非你电脑禁用IPV6<br />
<br />
国内的话IPV6也要比IPV4慢很多

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339579&amp;ptid=757469" target="_blank"><font color="#999999">ABCHINA 发表于 2020-10-23 09:47</font></a></font><br />
windows10如果有IPV6的话，浏览器什么的都会默认走IPV6出口（如果服务提供的话），很慢，真的垃圾。设置I ...</blockquote></div><br />
目前网站可能支持，但是设备估计没有全部支持IPV6，等全面普及看看速度。<br />
国家想弯道超车的，所以要政策推IPV6

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339444&amp;ptid=757469" target="_blank"><font color="#999999">shelizi1 发表于 2020-10-23 09:25</font></a></font><br />
网站支持V4和V6双栈访问，政府和事业单位要起带头作用。</blockquote></div><br />
你是运营商或者云商吧。。就是提供底层能力的。<br />
<br />
这个需要底层比如openstack改造，然后给虚机分配，然后对于具体程序配置文件增加v6内容，比如nginx的等，然后域名加上解析就可以了；

同样CC的机，V4 ping延迟170，V6延迟260

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339656&amp;ptid=757469" target="_blank"><font color="#999999">吾爱互联 发表于 2020-10-23 10:00</font></a></font><br />
你是运营商或者云商吧。。就是提供底层能力的。<br />
<br />
这个需要底层比如openstack改造，然后给虚机分配，然后 ...</blockquote></div><br />
运营商或者云商，现在开始都是直接更换设备支持IPV6了。<br />
<br />
老机房的是用翻译系统过渡，现场换成本毕竟大一些，要等计划，不过可有的等了。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339450&amp;ptid=757469" target="_blank"><font color="#999999">llmwxt 发表于 2020-10-23 09:27</font></a></font><br />
我觉得最重要的是，更好追踪！</blockquote></div><br />
V4也一样，我觉得可能是想弯道超车，不然跑不到前面去，所以才政策推进。
