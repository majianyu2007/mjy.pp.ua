# 发现Google Analyics的BUG


不知道有没有小伙伴发现&nbsp;&nbsp;Google Analyics展示的网站流量数据不太准确<br />
Zhengzhou的网站访问者 会识别成Hangzhou<br />
有知道怎么给Google提BUG的小伙伴吗？

EMAIL试试吧！<br />
<br />
<img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" />

这个是谷歌IP精度问题<img id="aimg_TJK3s" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

ip识别有问题，我的香港ip被谷歌识别成菲律宾了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

Google Analyics 会拖慢国内用户的访问速度吗 我想借楼问问

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375376&amp;ptid=760253" target="_blank"><font color="#999999">Cstudent 发表于 2020-10-30 15:07</font></a></font><br />
Google Analyics 会拖慢国内用户的访问速度吗 我想借楼问问</blockquote></div><br />
统计不会，广告会<img id="aimg_j1bhh" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375376&amp;ptid=760253" target="_blank"><font color="#999999">Cstudent 发表于 2020-10-30 15:07</font></a></font><br />
Google Analyics 会拖慢国内用户的访问速度吗 我想借楼问问</blockquote></div><br />
这个不清楚 没有做过对比实验 也许会拖慢个0.x秒吧

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375428&amp;ptid=760253" target="_blank"><font color="#999999">tdd 发表于 2020-10-30 15:17</font></a></font><br />
这个不清楚 没有做过对比实验 也许会拖慢个0.x秒吧</blockquote></div><br />
可以买个CDN

不是不准确，是非常不准确，我把后台的数据和GA统计数据用order id去筛选，猜猜丢失数据占比是多少。<br />
<br />
没错，有 45%-60%的数据是遗失的。。。<br />

