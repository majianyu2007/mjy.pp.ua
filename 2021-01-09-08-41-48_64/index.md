# IPV6网址升级改造有人接触过吗？


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339690&amp;ptid=757469" target="_blank"><font color="#999999">shelizi1 发表于 2020-10-23 10:05</font></a></font><br />
V4也一样，我觉得可能是想弯道超车，不然跑不到前面去，所以才政策推进。 ...</blockquote></div><br />
V4好一点的，内网就没办法确定了！

同城城域网 ipv4互访32ms ipv6互访12ms<br />
ipv6现阶段将处于并长期处于和ipv4并存的双栈阶段 但迟早有一天会大范围取代ipv4使用<img id="aimg_Zfwex" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339699&amp;ptid=757469" target="_blank"><font color="#999999">wqz 发表于 2020-10-23 10:06</font></a></font><br />
同城城域网 ipv4互访32ms ipv6互访12ms<br />
ipv6现阶段将处于并长期处于和ipv4并存的双栈阶段 但迟早有一天会大 ...</blockquote></div><br />
长期会很长，政策推进很难能完全实现。就看没有利益点爆发，让使用者完全过渡V6上。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339696&amp;ptid=757469" target="_blank"><font color="#999999">llmwxt 发表于 2020-10-23 10:06</font></a></font><br />
V4好一点的，内网就没办法确定了！</blockquote></div><br />
内网的，就物理上门。<img src="static/image/smiley/yct/010.gif" smilieid="41" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339668&amp;ptid=757469" target="_blank"><font color="#999999">微笑丶在脸上 发表于 2020-10-23 10:02</font></a></font><br />
同样CC的机，V4 ping延迟170，V6延迟260</blockquote></div><br />
都主要看机房设备支不支持V6的，目前看还不是很大规模，或者是线路不好。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339740&amp;ptid=757469" target="_blank"><font color="#999999">老坛酸菜 发表于 2020-10-23 10:11</font></a></font><br />
设备得同频吧 不然没意义</blockquote></div><br />
两种方式，一种就是机房全换支持V6设备。<br />
另外一种是给弄个翻译系统同步。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339677&amp;ptid=757469" target="_blank"><font color="#999999">shelizi1 发表于 2020-10-23 10:03</font></a></font><br />
运营商或者云商，现在开始都是直接更换设备支持IPV6了。<br />
<br />
老机房的是用翻译系统过渡，现场换成本毕竟大一 ...</blockquote></div><br />
设备几年前就支持，问题是虚拟化底层不支持，比如openstack K版等，另外就是平台侧不支持。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9340016&amp;ptid=757469" target="_blank"><font color="#999999">吾爱互联 发表于 2020-10-23 10:46</font></a></font><br />
设备几年前就支持，问题是虚拟化底层不支持，比如openstack K版等，另外就是平台侧不支持。 ...</blockquote></div><br />
大的机房换了，小的和老的就不好靠，运营商的流程慢的很，而且本身也有业务切换，运维技术反馈也慢。

ipv6和过去的网购一样，未来是趋势
