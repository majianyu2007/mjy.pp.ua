# 求解，Nginx反代遇到的问题


<i class="pstatus"> 本帖最后由 Feather 于 2020-10-28 18:13 编辑 </i><br />
<br />
一台服务器有5个IP，后面一群小鸡当反代，反代的都是服务器同一个IP，但是访问量多点的时候全都是504错误了，服务器上的没挂掉，然后前面一堆小鸡把反代的IP更改下又没这个问题了，端口开放了很多个，但是没卵用，只有小鸡那源站IP设置不同的才好使，哪位大佬帮忙解惑一下。<br />
------最终的原因找到了------<br />
Windows2008 R2 运行时间超过497天，TCP/IP的端口不再自动释放<br />
这个漏洞没更新，刚好服务器499天没关机了，也就是刚好前天开始的

TCP连接数的问题

帮顶，让技术大佬看到！<br />
<br />
<img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" />

504是代理服务器无法访问小鸡<img id="aimg_GatcC" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

有可能访问量大被后端防火墙识别为cc <img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><br />
当然也可以试试试试配置负载均衡 upstream

504是小鸡带宽不够，无法从杜甫获取数据，要不然杜甫的nginx小鸡反带是没问题的

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9364782&amp;ptid=759456" target="_blank"><font color="#999999">liuyangge 发表于 2020-10-28 16:47</font></a></font><br />
有可能访问量大被后端防火墙识别为cc <br />
当然也可以试试试试配置负载均衡 upstream ...</blockquote></div><br />
杜甫，就Windows自带的防火墙，所以不存在CC这个问题

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9364800&amp;ptid=759456" target="_blank"><font color="#999999">a87750530 发表于 2020-10-28 16:50</font></a></font><br />
504是小鸡带宽不够，无法从杜甫获取数据，要不然杜甫的nginx小鸡反带是没问题的 ...</blockquote></div><br />
也不是带宽不够，综合下来整个带宽使用率还不到3M/S，国外服务器来说，3M/S不到的使用率是超级低的了，但是只要不是都全部反代同一个IP，这个问题又没有了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9364810&amp;ptid=759456" target="_blank"><font color="#999999">Feather 发表于 2020-10-28 16:52</font></a></font><br />
也不是带宽不够，综合下来整个带宽使用率还不到3M/S，国外服务器来说，3M/S不到的使用率是超级低的了，但 ...</blockquote></div><br />
你换端口嘛，比如A--81端口<br />
B-82端口，再加上换ip不就解决了<br />
504很大问题是小鸡访问不了后端杜甫！不是杜甫本身问题

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9364824&amp;ptid=759456" target="_blank"><font color="#999999">a87750530 发表于 2020-10-28 16:54</font></a></font><br />
你换端口嘛，比如A--81端口<br />
B-82端口，再加上换ip不就解决了<br />
504很大问题是小鸡访问不了后端杜甫！不是杜 ...</blockquote></div><br />
端口每台小鸡反代源站都是用的不同端口，但是没卵用，只有用不同IP才行，所以费解的就是这点

起码你要把配置贴出来，不然鬼知道
