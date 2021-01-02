# docker想自己制作镜像的话推荐什么系统哇


<img src="static/image/smiley/yct/014.gif" smilieid="45" border="0" alt="" /> <br />
萌新想把自己常用的一些软件打包进去，但是不知道容器内啥系统比较好。<br />
<br />
貌似看见Alpine的比较多，还是说就搞个debian什么的。<br />
<br />
想知道有啥比较好用的。<br />


要看你制作什么功能的镜像了，alpine最小

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9397291&amp;ptid=761936" target="_blank"><font color="#999999">809509941 发表于 2020-11-3 18:26</font></a></font><br />
那有没有哪里有比较基础的debian系统镜像啊。我看官方的啥都要自己安装，好麻烦。 ...</blockquote></div><br />
<br />
<br />
pull debian:10<br />
<br />
以后不要问这种问题了，查手册

alpine包不全，debian/ubuntu

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9397270&amp;ptid=761936" target="_blank"><font color="#999999">h20 发表于 2020-11-3 18:24</font></a></font><br />
alpine包不全，debian/ubuntu</blockquote></div><br />
那有没有哪里有比较基础的debian系统镜像啊。我看官方的啥都要自己安装，好麻烦。<img src="static/image/smiley/yct/013.gif" smilieid="43" border="0" alt="" />

docker镜像肯定越小越好，首选alpine。

首选alpine，次选ubuntu、Debian。

只依赖自己脚本的话选alpine，有apt啥的直接进行一个ubuntu的选

你做点大众点的&nbsp;&nbsp;我也白**一下

越小越好。方便捏着带走。（数据肯定要在容器外。容器内数据只负责程序正常运行。<br />
我觉得按照这个思路的话……反而想要最小化的容器
