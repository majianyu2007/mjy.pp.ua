# 全球软路由论坛求解软路由的转发能力


我在想，G3220这个cpu能不能带满五个千兆网口啊？会不会出现CPU性能瓶颈。另外在没有VD-T的情况下，虚拟机下的pcie网卡会不会拉跨？

<i class="pstatus"> 本帖最后由 g6162227 于 2020-10-27 22:35 编辑 </i><br />
<br />
第一五个千兆就扯了，他又不是交换机，除非inbond大于5G，另外小包转发和内部横向流量交换软路由不行；第二 vt-d后你会发现没啥用。

你说的跑满，是直接路由转发，还是解析那啥？<br />
<br />
这个得说清楚啊！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

买个试试就知道了

我也想問，最近想用i9 9900k組軟路由+主動入侵防火牆。想問問10G網口能不能帶動?

软路由不要当成交换机用，LAN口有一个就行了，剩下的交给专业的交换机或AP来

即使是5个千兆难道使用的时候能一直跑满？<img id="aimg_zbr3I" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

自己搜koolshare 有专业帖子 小包很烂

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9361209&amp;ptid=759157" target="_blank"><font color="#999999">llmwxt 发表于 2020-10-27 20:59</font></a></font><br />
你说的跑满，是直接路由转发，还是解析那啥？<br />
<br />
这个得说清楚啊！</blockquote></div><br />
<br />
我是想PCIE插一个四口网卡，加上主板自带的一个，直接装上软路由当路由器+交换机使用。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9361670&amp;ptid=759157" target="_blank"><font color="#999999">g6162227 发表于 2020-10-27 22:33</font></a></font><br />
第一五个千兆就扯了，他又不是交换机，除非inbond大于5G，另外小包转发和内部横向流量交换软路由不行；第二 ...</blockquote></div><br />
好呢，最主要的还是内部横向流量交换。因为是台NAS，要看看电影的。
