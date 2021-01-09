# urlos居然不支持修改默认端口


买了两套的撸过。。。。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9381639&amp;ptid=760651" target="_blank"><font color="#999999">小穴儿 发表于 2020-10-31 19:11</font></a></font><br />
买了两套的撸过。。。。</blockquote></div><br />
然而有卵用没？<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

docker挺好用的，就是这个面板实在是有些鸡肋，实在需要面板可以试试portainer，我是觉得不错

哈哈哈 我特么买了6套吃灰玩

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9381668&amp;ptid=760651" target="_blank"><font color="#999999">zoenreo 发表于 2020-10-31 19:18</font></a></font><br />
docker挺好用的，就是这个面板实在是有些鸡肋，实在需要面板可以试试portainer，我是觉得不错 ...</blockquote></div><br />
太鸡儿坑了

最垃圾的是服务器必需内网，公网是无法使用的

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9381674&amp;ptid=760651" target="_blank"><font color="#999999">801N 发表于 2020-10-31 19:20</font></a></font><br />
最垃圾的是服务器必需内网，公网是无法使用的</blockquote></div><br />
我的就是NAT VPS，需要改指定端口才能访问，发工单告诉我，不支持修改端口，我丢

<i class="pstatus"> 本帖最后由 lovework 于 2020-11-1 11:58 编辑 </i><br />
<br />
回复楼主：<br />
<br />
由于LOC的帖子会被采集到别的网站，到处乱飞，所以还是回答一下：<br />
1. URLOS本身也以Docker容器的方式运行，可以任意修改9966和9968端口，只需要在执行docker run命令时执行时把服务端口修改掉即可（第二种安装URLOS的方法），如把9968和9966改为2268和2266：<br /><div class="blockcode"><div id="code_B9u"><ol><li>docker run -itd --name urlos --restart always -p 2268:9968 -p 2266:9966 -v /data/urlos:/data/urlos urlos/urlos</ol></div><em onclick="copycode($('code_B9u'));">复制代码</em></div><br />
2. 如果用我们的官方的安装脚本（第一种安装URLOS的方法），也可以在安装前执行以下代码把9968和9966改为2268和2266：<br /><div class="blockcode"><div id="code_V2g"><ol><li>export HTTP_PORT=2268 HTTPS_PORT=2266</ol></div><em onclick="copycode($('code_V2g'));">复制代码</em></div><br />
3. 系统设置中可以设置登录入口，如有兴趣，可以研究一下；<br />
4. URLOS可以在用完后直接关闭，用的时候再启动起来即可。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9381651&amp;ptid=760651" target="_blank"><font color="#999999">52naiba 发表于 2020-10-31 19:14</font></a></font><br />
然而有卵用没？</blockquote></div><br />
吃灰..别人有的 我一定要有。。。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9381674&amp;ptid=760651" target="_blank"><font color="#999999">801N 发表于 2020-10-31 19:20</font></a></font><br />
最垃圾的是服务器必需内网，公网是无法使用的</blockquote></div><br />
公网可以用，集群IP段设置为 0.0.0.0/0即可 
