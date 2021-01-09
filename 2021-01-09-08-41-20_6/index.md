# 请教一个PT下载的问题


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349387&amp;ptid=758239" target="_blank"><font color="#999999">gj368 发表于 2020-10-25 12:24</font></a></font><br />
上图床吧 我眼睛都要瞎了</blockquote></div><br />
不太会<img src="static/image/smiley/yct/014.gif" smilieid="45" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349442&amp;ptid=758239" target="_blank"><font color="#999999">无时崩溃 发表于 2020-10-25 12:38</font></a></font><br />
上图床 什么都看不清</blockquote></div><br />
不太会<img src="static/image/smiley/yct/014.gif" smilieid="45" border="0" alt="" />，全靠文字描述

10楼一语惊醒梦中人呀，大概率是文件夹权限问题。<br />
PT下载文件夹给777权限 chmod -R 777<img id="aimg_eXxvV" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349519&amp;ptid=758239" target="_blank"><font color="#999999">zaeve 发表于 2020-10-25 12:59</font></a></font><br />
10楼一语惊醒梦中人呀，大概率是文件夹权限问题。<br />
PT下载文件夹给777权限 chmod -R 777 ...</blockquote></div><br />
给了的，不行啊

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349410&amp;ptid=758239" target="_blank"><font color="#999999">shuohaobulude 发表于 2020-10-25 12:29</font></a></font><br />
论坛里有个组内网的帖子你搜一下</blockquote></div><br />
我是问你是咋组的 你这看起来好像是挂载大盘鸡到大流量鸡上了，估计是权限的问题 其实我感觉用大流量机做代理更方便点 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349536&amp;ptid=758239" target="_blank"><font color="#999999">dragonfsky 发表于 2020-10-25 13:05</font></a></font><br />
我是问你是咋组的 你这看起来好像是挂载大盘鸡到大流量鸡上了，估计是权限的问题 其实我感觉用大流量机做 ...</blockquote></div><br />
是的，挂载到流量鸡上

直接作弊，想啥呢，这么辣鸡，都过不了考核

chown -R transmission /pt目录<br />
chgrp -R transmission /pt目录

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349556&amp;ptid=758239" target="_blank"><font color="#999999">蝙蝠侠 发表于 2020-10-25 13:12</font></a></font><br />
chown -R transmission /pt目录<br />
chgrp -R transmission /pt目录</blockquote></div><br />
权限给了没用<img src="static/image/smiley/yct/021.gif" smilieid="37" border="0" alt="" />
