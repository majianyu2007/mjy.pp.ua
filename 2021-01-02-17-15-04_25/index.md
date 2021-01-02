# 云厂商用自建的DNS是真的坑


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347741&amp;ptid=758023" target="_blank"><font color="#999999">秋上书 发表于 2020-10-24 21:32</font></a></font><br />
公共dns限制请求次数？？？</blockquote></div><br />
这个说的是阿里云，当时爬虫出问题，打死也没想到是DNS的问题，搞了好长时间。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347724&amp;ptid=758023" target="_blank"><font color="#999999">问世间情为何物 发表于 2020-10-24 21:27</font></a></font><br />
张嘴就知道女票，女票个几把啊，你见哪个公共DNS收费了？</blockquote></div><br />
不说清楚，谁知道你说的是公共dns。<br />
公共就是大家用的。<br />
搞的都被别人限制请求次数，涉嫌攻击dns了，还有理了。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347817&amp;ptid=758023" target="_blank"><font color="#999999">斜阳晚暮 发表于 2020-10-24 21:44</font></a></font><br />
不说清楚，谁知道你说的是公共dns。<br />
公共就是大家用的。<br />
搞的都被别人限制请求次数，涉嫌攻击dns了，还有 ...</blockquote></div><br />
几秒钟一个请求攻击个JB？？？你家几秒一个请求叫攻击 ？啥都没搞清楚就瞎JB喷。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347825&amp;ptid=758023" target="_blank"><font color="#999999">问世间情为何物 发表于 2020-10-24 21:46</font></a></font><br />
几秒钟一个请求攻击个JB？？？你家几秒一个请求叫攻击 ？啥都没搞清楚就瞎JB喷。 ...</blockquote></div><br />
限制几秒钟一个请求次数，这样泼别人脏水前，怎么先说服自己相信的，当别人都是傻子？<br />
全国用的多了。不能用的程度，会运行这么些年。<br />
自己问题找不出来，就知道瞎喷。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347737&amp;ptid=758023" target="_blank"><font color="#999999">jqbaobao 发表于 2020-10-24 21:31</font></a></font><br />
https://dns.google/dns-query<br />
tls://dns.google<br />
https://dns.cloudflare.com/dns-query</blockquote></div><br />
我也建国一次，但是显示拦截了，实际没拦截，很迷

自建DNS方便开展VPC内网解析业务啊，就凭这点，各厂商没有理由不自建递归DNS吧<img id="aimg_u136t" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347856&amp;ptid=758023" target="_blank"><font color="#999999">斜阳晚暮 发表于 2020-10-24 21:50</font></a></font><br />
限制几秒钟一个请求次数，这样泼别人脏水前，怎么先说服自己相信的，当别人都是傻子？<br />
全国用的多了。不 ...</blockquote></div><br />
<br />
第一，你用PHP写个爬虫你试试处理一次请求得多少长时间。<br />
第二，我都说了是IP被DNS屏蔽，这就是问题，什么叫找不出来？<br />
第三，什么叫瞎喷？事情是我自己经历过的我清楚的很，反倒你是啥都没搞清楚就瞎JB喷吧？这是病，得治。<br />
<br />
几秒一次请求就被封如果不是我亲自经历过我也不会信。别拿自己脑袋去脑补自己没经历过的事情 。

<i class="pstatus"> 本帖最后由 问世间情为何物 于 2020-10-24 22:04 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347885&amp;ptid=758023" target="_blank"><font color="#999999">iks 发表于 2020-10-24 21:57</font></a></font><br />
自建DNS方便开展VPC内网解析业务啊，就凭这点，各厂商没有理由不自建递归DNS吧 ...</blockquote></div><br />
<br />
自建可以，别TM搞出问题来啊。<br />
<br />
发这帖子是因为，用CF解析的域名，在LINODE上，用LINODE自建的DNS，我忘了等了多久，几分钟十几分钟几十分钟都有可能，就是解析不出来。<br />
<br />
如果用8.8.8.8，CF解析的域名可以按秒级解析出来。<br />
<br />
<br />
爬虫导致被DNS封IP的问题，这么些年以来我只遇到过一次，就是阿里云自建的DNS。

新手上路<img id="aimg_iR3m3" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
