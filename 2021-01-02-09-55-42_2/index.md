# 请教个反代问题刁大的说下？


<i class="pstatus"> 本帖最后由 evils 于 2020-10-25 15:18 编辑 </i><br />
<br />
后端A服务器 1.1.1.1 hostloc.com<br />
前端B服务器 2.2.2.2 hostloc.com<br />
<br />
用户经过前端B服务器访问服务 怎么让B服务器拉A的数据反馈给用户 两个服务器必须绑定的域名一致<br />
<br />
<br />
原因是因为挂载了个网盘程序<br />
程序后台 要设置个域名访问&nbsp;&nbsp;<br />
然后我想反代一下这个域名<br />
<br />
zfile作者这样说的<br />
<br />
结果就是：下载的地址，取决于后台的站点设置中的域名。<br />
<br />
那里填写的地址，你可以经过反代，只要能被服务器访问到。

你直接说你要实现的目的，而不是你自己想的思路，我估计更容易解决问题

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349973&amp;ptid=758279" target="_blank"><font color="#999999">5000000 发表于 2020-10-25 15:09</font></a></font><br />
你直接说你要实现的目的，而不是你自己想的思路，我估计更容易解决问题</blockquote></div><br />
目的已经说了

人类迷惑行为

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349979&amp;ptid=758279" target="_blank"><font color="#999999">h20 发表于 2020-10-25 15:11</font></a></font><br />
人类迷惑行为</blockquote></div><br />
已更新问题

基础应用。。。看一遍nginx的proxy规则直接写就行了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9350102&amp;ptid=758279" target="_blank"><font color="#999999">风筝于风 发表于 2020-10-25 15:41</font></a></font><br />
基础应用。。。看一遍nginx的proxy规则直接写就行了</blockquote></div><br />
不会搞
