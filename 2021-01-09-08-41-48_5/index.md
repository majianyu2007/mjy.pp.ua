# 腾讯云香港轻量。宝塔装了系统防火墙后打不开了


ssh输入<div class="blockcode"><div id="code_feH"><ol><li>firewall-cmd --list-all</ol></div><em onclick="copycode($('code_feH'));">复制代码</em></div>看看

你ssh端口改了吗？

<div class="quote"><blockquote><font color="#999999">kra 发表于 2020-10-28 18:52</font><br />
<font color="#999999">centos&nbsp;&nbsp;有得玩了。<br />
开启firewall，又没开放端口，直接堵上了。。。</font></blockquote></div><br />
当年就是这个原因，centos弃了

宝塔修改过后台端口<br />
但是你防火墙忘记放心了<br />
<br />
ssh链接上去&nbsp;&nbsp;输入 bt<br />
看看能不能清除一下

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9365791&amp;ptid=759514" target="_blank"><font color="#999999">炮姐的安全裤 发表于 2020-10-28 19:27</font></a></font><br />
当年就是这个原因，centos弃了</blockquote></div><br />
哈哈，确实有坑，又得通过网页端ssh连上修改。。。<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" />

解决了，谢谢大家。防火墙是宝塔的插件，我重启了轻量的服务器就可以访问了
