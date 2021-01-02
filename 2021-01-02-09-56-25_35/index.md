# PR技术让帮忙问一下


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9412425&amp;ptid=763264" target="_blank"><font color="#999999">开腥小站长 发表于 2020-11-6 15:24</font></a></font><br />
严格来说ST（系统负载占用）应该区于0-0.5之间……</blockquote></div><br />
那没办法，我自买来ST几乎就在5左右，后来降到5以下，现在最高也超不出5。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9412290&amp;ptid=763264" target="_blank"><font color="#999999">laogui 发表于 2020-11-6 15:03</font></a></font><br />
让技术解释解释，每天白白跑4G多的流量<br />
一个月下来，白白浪费120多G流量<br />
虽然放着吃灰，但是也无比心痛</blockquote></div><br />
这是哪个命令

15点37分（CST）开始负载明显下降，但ARP包仍然不断，网络性能没有明显的改善<img id="aimg_s1q2g" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 眷恋 于 2020-11-6 16:44 编辑 </i><br />
<br />
看不懂，随便Ping了下，但是偷跑流量还在继续<br />
补充下，1号母鸡<br />
<img id="aimg_pz5G8" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/11/06/lkAjmvT3Q2erZHn.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

老affman已跳车 <img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9412275&amp;ptid=763264" target="_blank"><font color="#999999">开腥小站长 发表于 2020-11-6 03:01</font></a></font><br />
老PR，新的没这问题</blockquote></div><br />
怎么分变新老

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9412838&amp;ptid=763264" target="_blank"><font color="#999999">斌斌 发表于 2020-11-6 16:33</font></a></font><br />
这是哪个命令</blockquote></div><br />
<br />
vnstat<br />
搜索下，然后安装

我啥也没干，显示9天跑了24个G<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><br />
<img id="aimg_kftxF" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/11/06/BhV2Af.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

vnstat -l<br />
Monitoring eth0...&nbsp; &nbsp; (press CTRL-C to stop)<br />
<br />
&nbsp; &nbsp;rx:&nbsp; &nbsp;168.83 kbit/s&nbsp; &nbsp;298 p/s&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; tx:&nbsp; &nbsp;&nbsp;&nbsp;1.49 kbit/s&nbsp; &nbsp;&nbsp;&nbsp;2 p/s^C<br />
<br />
<br />
 eth0&nbsp;&nbsp;/&nbsp;&nbsp;traffic statistics<br />
<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;rx&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;|&nbsp; &nbsp;&nbsp; &nbsp; tx<br />
--------------------------------------+------------------<br />
&nbsp;&nbsp;bytes&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;2.39 MiB&nbsp;&nbsp;|&nbsp; &nbsp;&nbsp; &nbsp; 17.52 KiB<br />
--------------------------------------+------------------<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; max&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 226.06 kbit/s&nbsp;&nbsp;|&nbsp; &nbsp;&nbsp;&nbsp;3.06 kbit/s<br />
&nbsp; &nbsp;&nbsp; &nbsp;average&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 142.94 kbit/s&nbsp;&nbsp;|&nbsp; &nbsp;&nbsp;&nbsp;1.02 kbit/s<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; min&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;22.42 kbit/s&nbsp;&nbsp;|&nbsp; &nbsp;&nbsp; &nbsp; 168 bit/s<br />
--------------------------------------+------------------<br />
&nbsp;&nbsp;packets&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 38103&nbsp;&nbsp;|&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 130<br />
--------------------------------------+------------------<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; max&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 360 p/s&nbsp;&nbsp;|&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;4 p/s<br />
&nbsp; &nbsp;&nbsp; &nbsp;average&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 272 p/s&nbsp;&nbsp;|&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;0 p/s<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; min&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;46 p/s&nbsp;&nbsp;|&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;0 p/s<br />
--------------------------------------+------------------<br />
&nbsp;&nbsp;time&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;2.33 minutes<br />
<br />
还是和以前一样

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9412290&amp;ptid=763264" target="_blank"><font color="#999999">laogui 发表于 2020-11-6 15:03</font></a></font><br />
让技术解释解释，每天白白跑4G多的流量<br />
一个月下来，白白浪费120多G流量<br />
虽然放着吃灰，但是也无比心痛</blockquote></div><br />
 ------------------------+-------------+-------------+---------------<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月08日&nbsp; &nbsp; 8.03 GiB |&nbsp; &nbsp; 2.38 GiB |&nbsp; &nbsp;10.41 GiB |&nbsp; &nbsp; 1.04 Mbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月09日&nbsp; &nbsp; 5.55 GiB |&nbsp; &nbsp;77.90 MiB |&nbsp; &nbsp; 5.63 GiB |&nbsp;&nbsp;559.76 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月10日&nbsp; &nbsp; 5.44 GiB |&nbsp;&nbsp;122.30 MiB |&nbsp; &nbsp; 5.55 GiB |&nbsp;&nbsp;552.27 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月11日&nbsp; &nbsp; 5.50 GiB |&nbsp;&nbsp;315.73 MiB |&nbsp; &nbsp; 5.81 GiB |&nbsp;&nbsp;577.27 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月12日&nbsp; &nbsp; 5.46 GiB |&nbsp; &nbsp;16.99 MiB |&nbsp; &nbsp; 5.48 GiB |&nbsp;&nbsp;544.45 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月13日&nbsp; &nbsp; 5.50 GiB |&nbsp; &nbsp; 7.05 MiB |&nbsp; &nbsp; 5.51 GiB |&nbsp;&nbsp;547.99 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月14日&nbsp; &nbsp; 5.61 GiB |&nbsp; &nbsp;50.84 MiB |&nbsp; &nbsp; 5.66 GiB |&nbsp;&nbsp;562.30 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月15日&nbsp; &nbsp; 5.30 GiB |&nbsp; &nbsp;39.98 MiB |&nbsp; &nbsp; 5.33 GiB |&nbsp;&nbsp;530.39 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月16日&nbsp; &nbsp; 5.30 GiB |&nbsp; &nbsp;68.74 MiB |&nbsp; &nbsp; 5.36 GiB |&nbsp;&nbsp;533.18 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月17日&nbsp; &nbsp; 5.28 GiB |&nbsp; &nbsp; 7.88 MiB |&nbsp; &nbsp; 5.29 GiB |&nbsp;&nbsp;525.50 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月18日&nbsp; &nbsp; 5.26 GiB |&nbsp; &nbsp;59.82 MiB |&nbsp; &nbsp; 5.31 GiB |&nbsp;&nbsp;528.41 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月19日&nbsp; &nbsp; 5.07 GiB |&nbsp; &nbsp;28.62 MiB |&nbsp; &nbsp; 5.09 GiB |&nbsp;&nbsp;506.52 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月20日&nbsp; &nbsp; 4.97 GiB |&nbsp; &nbsp;58.29 MiB |&nbsp; &nbsp; 5.03 GiB |&nbsp;&nbsp;499.82 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月21日&nbsp; &nbsp; 4.72 GiB |&nbsp; &nbsp; 5.20 MiB |&nbsp; &nbsp; 4.72 GiB |&nbsp;&nbsp;469.49 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月22日&nbsp; &nbsp; 4.84 GiB |&nbsp; &nbsp; 4.29 MiB |&nbsp; &nbsp; 4.84 GiB |&nbsp;&nbsp;481.32 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月23日&nbsp; &nbsp; 5.00 GiB |&nbsp;&nbsp;252.96 MiB |&nbsp; &nbsp; 5.24 GiB |&nbsp;&nbsp;521.46 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月24日&nbsp; &nbsp; 5.85 GiB |&nbsp; &nbsp; 1.16 GiB |&nbsp; &nbsp; 7.01 GiB |&nbsp;&nbsp;696.95 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月25日&nbsp; &nbsp; 4.81 GiB |&nbsp; &nbsp;30.00 MiB |&nbsp; &nbsp; 4.84 GiB |&nbsp;&nbsp;480.87 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月26日&nbsp; &nbsp; 6.07 GiB |&nbsp; &nbsp; 1.38 GiB |&nbsp; &nbsp; 7.45 GiB |&nbsp;&nbsp;740.75 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月27日&nbsp; &nbsp; 6.88 GiB |&nbsp; &nbsp; 1.84 GiB |&nbsp; &nbsp; 8.73 GiB |&nbsp;&nbsp;867.59 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月28日&nbsp; &nbsp; 5.46 GiB |&nbsp;&nbsp;286.73 MiB |&nbsp; &nbsp; 5.74 GiB |&nbsp;&nbsp;570.85 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月29日&nbsp; &nbsp; 5.57 GiB |&nbsp;&nbsp;253.47 MiB |&nbsp; &nbsp; 5.82 GiB |&nbsp;&nbsp;578.66 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月30日&nbsp; &nbsp; 5.41 GiB |&nbsp; &nbsp; 4.62 MiB |&nbsp; &nbsp; 5.42 GiB |&nbsp;&nbsp;538.44 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年10月31日&nbsp; &nbsp; 5.70 GiB |&nbsp; &nbsp;12.97 MiB |&nbsp; &nbsp; 5.71 GiB |&nbsp;&nbsp;568.13 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年11月01日&nbsp; &nbsp;12.04 GiB |&nbsp; &nbsp; 6.24 GiB |&nbsp; &nbsp;18.28 GiB |&nbsp; &nbsp; 1.82 Mbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年11月02日&nbsp; &nbsp; 7.57 GiB |&nbsp; &nbsp; 4.30 GiB |&nbsp; &nbsp;11.87 GiB |&nbsp; &nbsp; 1.18 Mbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年11月03日&nbsp; &nbsp; 5.27 GiB |&nbsp;&nbsp;108.47 MiB |&nbsp; &nbsp; 5.38 GiB |&nbsp;&nbsp;534.60 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年11月04日&nbsp; &nbsp; 5.59 GiB |&nbsp;&nbsp;126.19 MiB |&nbsp; &nbsp; 5.72 GiB |&nbsp;&nbsp;568.23 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年11月05日&nbsp; &nbsp; 5.51 GiB |&nbsp; &nbsp;58.38 MiB |&nbsp; &nbsp; 5.57 GiB |&nbsp;&nbsp;553.43 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;2020年11月06日&nbsp;&nbsp;330.27 MiB |&nbsp;&nbsp;893.73 KiB |&nbsp;&nbsp;331.14 MiB |&nbsp;&nbsp;156.94 kbit/s<br />
&nbsp; &nbsp;&nbsp;&nbsp;------------------------+-------------+-------------+---------------<br />
<br />
彼此彼此，一天跑5个G。。。
