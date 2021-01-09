# 有没有java版的探针啊


 都是php的。还要部署php环境和nginx才能用&nbsp;&nbsp;<br />
<br />
耦合太高了<br />
<br />
<br />
就不能像java一样 一个jar包就能搞定吗<br />
<br />
<br />
有jar或war包的探针吗

安装JRE也是个大工程，<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359209&amp;ptid=758983" target="_blank"><font color="#999999">1号城管 发表于 2020-10-27 14:39</font></a></font><br />
安装JRE也是个大工程，</blockquote></div><br />
<br />
不用吧 rpm&nbsp;&nbsp;直接运行jdk包 自动配置环境变量路径&nbsp; &nbsp; 直接就能食用吧

这就要探讨到最好的语言了 <img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359235&amp;ptid=758983" target="_blank"><font color="#999999">Alicloud 发表于 2020-10-27 14:42</font></a></font><br />
这就要探讨到最好的语言了</blockquote></div><br />
卧槽！卧槽，卧槽卧槽<img src="static/image/smiley/yct/011.gif" smilieid="33" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359209&amp;ptid=758983" target="_blank"><font color="#999999">1号城管 发表于 2020-10-27 14:39</font></a></font><br />
安装JRE也是个大工程，</blockquote></div><br />
自己好好想想，PHP不过集成了一键安装，<br />
java更简单，直接wget 下载jdk1.8_xxx-linux.tar.gz<br />
tar -zxvf jdk*<br />
echo &quot;export&nbsp;&nbsp;JAVA_HOME=/path/jdk1.8_xxx&quot; &gt;/etc/profile<br />
echo &quot;export&nbsp;&nbsp;PATH=$JAVA_HOME/bin<img src="static/image/smiley/default/shy.gif" smilieid="8" border="0" alt="" />PATH&quot; &gt;/etc/profile<br />
source /etc/profile&nbsp;&nbsp;<br />
就完事了，完全不用编译等等。<br />
把这个集成脚本，分分钟秒杀PHP

<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" /> java更简单，springboot内置tomcat，直接java -jar一键启动

 py那不是更快?懒就上docker 

帮顶，NGINX不会和那啥一起配置，就只能放弃探针了！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359209&amp;ptid=758983" target="_blank"><font color="#999999">1号城管 发表于 2020-10-27 14:39</font></a></font><br />
安装JRE也是个大工程，</blockquote></div><br />
jre简单的一比啊<br />
<br />
apt install java就完事了
