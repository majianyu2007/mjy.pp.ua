# {已解决}老师傅，老问题：ssh通，ping通，是不是阻断了


<i class="pstatus"> 本帖最后由 战神赵日天 于 2020-10-27 22:06 编辑 </i><br />
<br />
一个小鸡，昨天开始无法油管<br />
ssh通，ping通&nbsp;&nbsp;，今天换了个端口重装，还是无法油管，不知道是不是阻断了，ion的<br />
<br />
<br />
额，换了centos7，也换了端口，。貌似centos8必须要开启端口才行，额，反正目前ok了

SSH通，那应该就不是墙啊！<br />
<br />
<img src="static/image/smiley/default/shocked.gif" smilieid="6" border="0" alt="" /><img src="static/image/smiley/default/shocked.gif" smilieid="6" border="0" alt="" /><img src="static/image/smiley/default/shocked.gif" smilieid="6" border="0" alt="" />

继续换端口啊 多换几个试一试

tcping试下，墙都是tcp阻断

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9361109&amp;ptid=759146" target="_blank"><font color="#999999">Bill_Carson 发表于 2020-10-27 20:43</font></a></font><br />
tcping试下，墙都是tcp阻断</blockquote></div><br />
用ping。chinaz，tcping有地址不

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9361113&amp;ptid=759146" target="_blank"><font color="#999999">战神赵日天 发表于 2020-10-27 20:44</font></a></font><br />
用ping。chinaz，tcping有地址不</blockquote></div><br />
https://www.toolsdaquan.com/ipcheck/<br />
直接测你的那啥端口

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9361119&amp;ptid=759146" target="_blank"><font color="#999999">Bill_Carson 发表于 2020-10-27 20:45</font></a></font><br />
https://www.toolsdaquan.com/ipcheck/<br />
直接测你的那啥端口</blockquote></div><br />
兄弟，我有点蒙蔽了，下面是结果，但是我ssh没问题啊，要是说没开放端口，ion也不需要啊。。，。要说是被墙了，那国外至少可以tcp啊<br />
<br />
国内检测结果：<br />
ICMP可用；TCP不可用<br />
<br />
国外检测结果：<br />
ICMP可用；TCP不可用

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9361199&amp;ptid=759146" target="_blank"><font color="#999999">战神赵日天 发表于 2020-10-27 20:57</font></a></font><br />
兄弟，我有点蒙蔽了，下面是结果，但是我ssh没问题啊，要是说没开放端口，ion也不需要啊。。，。要说是被 ...</blockquote></div><br />
国内国外都不能用是不是没开放端口

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9361268&amp;ptid=759146" target="_blank"><font color="#999999">shuke 发表于 2020-10-27 21:13</font></a></font><br />
国内国外都不能用是不是没开放端口</blockquote></div><br />
ion以前不用开放端口啊，蛋疼。。

<i class="pstatus"> 本帖最后由 kra 于 2020-10-27 21:53 编辑 </i><br />
<br />
能ssh连接，说明ip还正常<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />。<br />
ssh对应端口必是国内（外）tcp正常的。<br />
<br />
其他端口，若仍有国内外tcp不通，有以下可能：<br />
1.那个检查的端口没有被使用，或没有进程在使用，或进程异常退出。<br />
<br />
2.vps防火墙问题，未开端口，一般是centos 7类的系统，默认安装并启用防火墙。<br />
但debian 、ubuntu 没有安装防火墙，不用关心，可忽略此条。<br />
<br />
<br />
3.网页端防火墙开放的问题，一般是发生在谷歌云 阿里云等有此类控制面板的主机商。。。，非此类可忽略。
