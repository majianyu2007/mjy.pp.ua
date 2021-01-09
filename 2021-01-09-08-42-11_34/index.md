# aws lightsail昨天还能登陆，今天就登陆不了是什么鬼


aws lightsail昨天还能登陆，今天就登陆不了是什么鬼<br />
默认证书登陆，用了一年多了，昨天安装了docker<br />
现在BT面板还能登陆，但是ssh登陆不了<br />
第二次遇到这种问题，以前一台直接删了<br />
<br />
/home/ubuntu/.ssh<br />
看证书公钥在里面的 <br />
有没有大佬遇到过这种情况

自己把机器搞坏了，与lightsail有什么关系

首先你得搞清楚 是你得Linux 不能登录而不是 aws lightsail 不能登录，这样问问题才知道你还知道什么是什么。

<div class="quote"><blockquote>昨天安装了docker</blockquote></div><br />
<br />
那你还打那么多字问什么呢

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9380073&amp;ptid=760547" target="_blank"><font color="#999999">allnetstore 发表于 2020-10-31 12:21</font></a></font><br />
那你还打那么多字问什么呢</blockquote></div><br />
跟docker有关系吗？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9380066&amp;ptid=760547" target="_blank"><font color="#999999">jarvan 发表于 2020-10-31 12:19</font></a></font><br />
首先你得搞清楚 是你得Linux 不能登录而不是 aws lightsail 不能登录，这样问问题才知道你还知道什么是什么 ...</blockquote></div><br />
是Linux不能登陆 Ubuntu

有可能机器ip或者22端口被墙了

home目录被格了或者挂载了，公钥就不行了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9380087&amp;ptid=760547" target="_blank"><font color="#999999">xshell 发表于 2020-10-31 12:25</font></a></font><br />
是Linux不能登陆 Ubuntu</blockquote></div><br />
去看看22端口是否开了&nbsp; &nbsp;http://port.ping.pe/&nbsp; &nbsp;

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9380173&amp;ptid=760547" target="_blank"><font color="#999999">jarvan 发表于 2020-10-31 12:51</font></a></font><br />
去看看22端口是否开了&nbsp; &nbsp;http://port.ping.pe/</blockquote></div><br />
开了，正常连接，就是显示这个证书登录不了
