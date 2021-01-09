# 各位求救啊，IPTABLES的！！！


哈哈，我调试网站的时候就是这么干的谁都访问不了避免了遭受攻击。代码东拼西凑一下就好百度是万能的<img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" />

不错，，，技术贴~~

你这是生了多少小号啊，都打回金牌会员了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9341463&amp;ptid=757601" target="_blank"><font color="#999999">bobbylong 发表于 2020-10-23 15:35</font></a></font><br />
你这是生了多少小号啊，都打回金牌会员了</blockquote></div><br />
挺多的，一排排的

对于80端口可以，对于https这种办**直接被浏览器拦截<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />，除非你有google.com的证书<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />，所以不要想太多，直接drop掉不让访问最方便<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img id="aimg_gAHPC" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

 不错，，，技术贴~~

是不是可以在本机设置错误的dns解析 /etc/hosts&nbsp; &nbsp;&nbsp; &nbsp;<img src="static/image/smiley/yct/010.gif" smilieid="41" border="0" alt="" />把禁止用户访问的网址全部解析到一个单独的网站

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9341267&amp;ptid=757601" target="_blank"><font color="#999999">芭啦啦能量 发表于 2020-10-23 15:01</font></a></font><br />
要求：请求服务器A的80，由A转到服务器B<br />
环境：<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;A：iptables&nbsp; &nbsp;google.com</blockquote></div><br />
学一招<img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" /><img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" />
