# 询问linux命令问题


<i class="pstatus"> 本帖最后由 vanilla 于 2020-10-22 20:59 编辑 </i><br />
<br />
这个一个dockerfile<br /><div class="blockcode"><div id="code_Inp"><ol><li>FROM i386/alpine:edge<br /><li>ENV GLIB_VERSION=2.26-6 GLIB_ARCH=i686 PYTHONUNBUFFERED=1<br /><li>RUN apk update &amp;&amp; apk add --no-cache \<br /><li>&nbsp; &nbsp; tar \<br /><li>&nbsp; &nbsp; procps \<br /><li>&nbsp; &nbsp; findutils \<br /><li>&nbsp; &nbsp; grep&nbsp;&nbsp;\<br /><li>&nbsp; &nbsp; tzdata \<br /><li>&nbsp; &nbsp; python3 \&nbsp; &nbsp;<br /><li>&nbsp; &nbsp; py3-pip \<br /><li>&nbsp; &nbsp; bash \<br /><li>&nbsp; &nbsp; curl \<br /><li>&nbsp; &nbsp; rclone \<br /><li>&nbsp; &nbsp; zlib \<br /><li>&nbsp; &nbsp; libgcc \<br /><li>&nbsp; &nbsp; ts \<br /><li>&nbsp; &nbsp; openssh &amp;&amp; \<br /><li>&nbsp; &nbsp; apk add --no-cache --virtual .build-dependencies \<br /><li>&nbsp; &nbsp; python3-dev \<br /><li>&nbsp; &nbsp; libevent-dev \<br /><li>&nbsp; &nbsp; gcc \<br /><li>..........<br /><li><br /><li><br /><li></ol></div><em onclick="copycode($('code_Inp'));">复制代码</em></div><br />
<br />
想问下这里面这个ts的shell命令是怎么单独在centos或者debian安装的？到处查都找不到这是个什么，apt，yum安装也没办法安装。。。

moreutils 工具包有ts，安装它就行。<br />
<br />
就好像net-tools工具包有netstat，安装它就可以用netstat

技术白路过帮顶！<br />
<br />
等大佬们回答！<br />
<br />
<img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" /><img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" /><img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" />

apk add ts<br />
<br />
https://alpine.pkgs.org/edge/alpine-community-x86/ts-1.0-r1.apk.html

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9337978&amp;ptid=757350" target="_blank"><font color="#999999">Firedoge 发表于 2020-10-22 20:57</font></a></font><br />
apk add ts<br />
<br />
https://alpine.pkgs.org/edge/alpine-community-x86/ts-1.0-r1.apk.html</blockquote></div><br />
我也找到这个，但是这个到底是什么呢。。centos和debian要怎么安装呢

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9337980&amp;ptid=757350" target="_blank"><font color="#999999">vanilla 发表于 2020-10-22 00:58</font></a></font><br />
我也找到这个，但是这个到底是什么呢。。centos和debian要怎么安装呢</blockquote></div><br />
<br />
自己下载编译<br />
https://vicerveza.homeunix.net/~viric/soft/ts/ts-1.0.tar.gz<br />
<br />
Debian下叫 task-spooler

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9337988&amp;ptid=757350" target="_blank"><font color="#999999">Firedoge 发表于 2020-10-22 21:01</font></a></font><br />
自己下载编译<br />
https://vicerveza.homeunix.net/~viric/soft/ts/ts-1.0.tar.gz</blockquote></div><br />
<img src="static/image/smiley/yct/002.gif" smilieid="30" border="0" alt="" />好吧

apt-get install moreutils

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9337988&amp;ptid=757350" target="_blank"><font color="#999999">Firedoge 发表于 2020-10-22 21:01</font></a></font><br />
自己下载编译<br />
https://vicerveza.homeunix.net/~viric/soft/ts/ts-1.0.tar.gz</blockquote></div><br />
哦哦，感谢感谢

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9338020&amp;ptid=757350" target="_blank"><font color="#999999">caddy 发表于 2020-10-22 21:05</font></a></font><br />
apt-get install moreutils</blockquote></div><br />
感谢感谢
