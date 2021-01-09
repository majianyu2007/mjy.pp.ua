# 求解，Nginx反代遇到的问题


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9364833&amp;ptid=759456" target="_blank"><font color="#999999">Feather 发表于 2020-10-28 16:55</font></a></font><br />
端口每台小鸡反代源站都是用的不同端口，但是没卵用，只有用不同IP才行，所以费解的就是这点 ...</blockquote></div><br />
504之前我也碰到过，也是前端反带后端，问题根源就是小鸡带宽不够，访问不了母鸡，换小鸡解决

TCP连接数的问题

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9364948&amp;ptid=759456" target="_blank"><font color="#999999">lijihede 发表于 2020-10-28 17:06</font></a></font><br />
TCP连接数的问题</blockquote></div><br />
netstat -ano看了下，爆表了
