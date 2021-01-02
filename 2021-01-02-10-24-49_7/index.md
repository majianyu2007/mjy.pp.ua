# EHEH.通知:因Cloudraft的故障导致的监控可能存在漏报的通知


<i class="pstatus"> 本帖最后由 superEric 于 2021-1-2 09:29 编辑 </i><br />
<br />
因CloudRaft提供的cfp业务故障导致可能有问题<br />
发布于2021年01月02日<br />
<br />
<font color="Red">新年第二天，给大家拜个早年。</font><br />
<br />
<br />
早上6点多接 提供Cloudflare partner 业务的CloudRaft 公司邮件，因该公司迁移数据误操作，导致已接入的所有用户数据和产品数据丢失。需要紧急修复。<br />
<br />
eheh早上8点多看到邮件，已经第一时间做了迁移。并在迁移之前做了部分测试，<font color="Red">eheh.org的网站监控依然运行正常！观测到的数据是6点多到8点之间，10台观测服务器数据运行正常。上报正常。监控正常。</font><br />
<br />
但依然存在某种可能：某些地区服务器上传的数据因此故障导致上传失败，进而报警。请大家忽略该报警信息。EHEH将继续给大家提供服务，并根据此故障，<font color="Red">在下个版本增加负载均衡和区域线路，来确保故障容灾！客户端则追加本地存储等功能。目前所有有服务器监控着的在用用户依然免费享用 </font><br />
<br />
对已有影响的用户朋友们，敬请谅解！<br />
<br />
<br />
------------<br />
<font color="Red"><font size="4">新年广告第一发：&nbsp;&nbsp;eheh.org  提供免费的Linux服务器性能监控和免费的ssl证书过期监控。&nbsp; &nbsp;我们轻量，一句话安装，同时我们是认真的，朝着专业方向发展。&nbsp;&nbsp;诚邀2021 各位 yjj 人士试用</font></font><br />
<br />


支持，正在使用

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9780147&amp;ptid=791763" target="_blank"><font color="#999999">fenglin2020 发表于 2021-1-2 09:15</font></a></font><br />
支持，正在使用</blockquote></div><br />
感谢老铁！！如有问题，随时跟我们说下！

<div class="quote"><blockquote>eheh.org&nbsp;&nbsp;提供免费的Linux服务器性能监控和免费的ssl证书过期监控。</blockquote></div><img id="aimg_tx2my" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

帮顶，在使用<img id="aimg_c3T96" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9780192&amp;ptid=791763" target="_blank"><font color="#999999">qer 发表于 2021-1-2 09:29</font></a></font><br />
帮顶，在使用</blockquote></div><br />
新年大吉，感恩：） 
