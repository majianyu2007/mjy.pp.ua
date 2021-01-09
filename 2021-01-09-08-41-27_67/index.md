# forwordpanel闲蛋中转面板 1.0.2版 docker导出镜像


https://mega.nz/file/yWAAlRbQ#M3y2Jlyt54nnHuPoHnRk167ZP_VXrLaHNvrFb_kNSa0<br />
从vps里导出的，方便需要的人。<br />
下载到vps里<br />
执行 docker load -i forwordpanel.tar 导入<br />
之后 docker images 查看 <font color="Red">IMAGE ID</font><br />
<br />
docker run --restart=always --name <font color="RoyalBlue">forwordpanel</font> -p <font color="RoyalBlue">12345</font>:8080 -d <font color="Red">d814e2078ef5</font><br />
<br />
自己改成想要设置的<font color="RoyalBlue">名字</font>和<font color="RoyalBlue">端口</font>。<font color="Red">d814e2078ef5</font>换成自己的<font color="Red">IMAGE ID</font><br />
<br />
访问IP:<font color="RoyalBlue">端口</font><br />
默认用户admintest<br />
密码admintest

我fork了一份。。<br />
<br />
https://github.com/yanaxiao/forwordpanel

马克~

没用过，使用效果如何

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351794&amp;ptid=758404" target="_blank"><font color="#999999">laogui 发表于 2020-10-25 23:08</font></a></font><br />
没用过，使用效果如何</blockquote></div><br />
使用iptables转发，一般。<br />
入门级操作，适合新手

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351755&amp;ptid=758404" target="_blank"><font color="#999999">yanaxiao 发表于 2020-10-25 23:00</font></a></font><br />
我fork了一份。。<br />
<br />
https://github.com/yanaxiao/forwordpanel</blockquote></div><br />
感谢大佬。。已fork

最新是不是1.0.3

最新的稳定版是1.0.7吧

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354197&amp;ptid=758404" target="_blank"><font color="#999999">twiter 发表于 2020-10-26 14:55</font></a></font><br />
最新的稳定版是1.0.7吧</blockquote></div><br />
我没更新。没有
