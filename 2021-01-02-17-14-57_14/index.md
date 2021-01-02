# 腾讯云服务器 公众号，发的那个图片什么意思？ 怎么解析？


54，68，65<br />
62，65，73，74<br />
77，61，79<br />
74，6F<br />
....<br />
<br />
<br />
<br />
怎么翻译？

The best way to predict future is to create it

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9344721&amp;ptid=757889" target="_blank"><font color="#999999">silence 发表于 2020-10-24 10:38</font></a></font><br />
The best way to predict future is to create it</blockquote></div><br />
什么方法翻译的？<img id="aimg_P34oC" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

很简单，我一开始猜测是asc2，但事实上不是，单纯用asc2解决只会得到乱码<br />
仔细看了下整段代码，发现6F,没有超出F的记录，典型的16进制<br />
我中间试了转2进制没有头绪<br />
然后用16进制转10进制，<br />
54，68，65 =84, 104，101<br />
对应asc2表 84, 104，101 = T,h,e<br />
出了正常单词了，所以以此类推就完事了，2楼已经把结果说出来了<br />

