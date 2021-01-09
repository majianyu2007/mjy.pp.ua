# Win10自带的杀毒真的是不行


1. 先用C#写了一个定时截屏上传到指定地址的后台程序,<br />
&nbsp; &nbsp; &nbsp; &nbsp; Windows 10 defender：未报毒<br />
&nbsp; &nbsp; &nbsp; &nbsp; 卡巴斯基： 报毒<br />
&nbsp; &nbsp; &nbsp; &nbsp; Eset：报毒<br />
<br />
2. 然后写了一个记录键盘的钩子：<br />
&nbsp; &nbsp; &nbsp; &nbsp; Windows 10 defender：未报毒<br />
&nbsp; &nbsp; &nbsp; &nbsp; 卡巴斯基： 报毒<br />
&nbsp; &nbsp; &nbsp; &nbsp; Eset：报毒<br />
<br />
3. 将上面两个加上自启动<br />
&nbsp; &nbsp; &nbsp; &nbsp; Windows 10 defender：报毒<br />
&nbsp; &nbsp; &nbsp; &nbsp; 卡巴斯基： 报毒<br />
&nbsp; &nbsp; &nbsp; &nbsp; Eset：报毒<br />
<br />
4. 写了个恶搞程序，运行后生成一个格式化所有硬盘的批处理文件，然后运行。<br />
&nbsp; &nbsp; &nbsp; &nbsp; Windows 10 defender：未报毒<br />
&nbsp; &nbsp; &nbsp; &nbsp; 卡巴斯基： 报毒<br />
&nbsp; &nbsp; &nbsp; &nbsp; Eset：报毒<br />
<br />
结论：Windows defender真的就是玩玩而已，普普通通用电脑的人倒无所谓。如果真被有心人盯上了，Defender真是无能为力。

<i class="pstatus"> 本帖最后由 龟龟酱 于 2020-10-26 18:04 编辑 </i><br />
<br />
不是windows defender只能玩玩而已<br />
是你的做法是玩玩而已...<br />
WD非常依赖云,而不是启发,所以会在你把这个样本发出去之后很快的拉黑,而不是在你自己测试的时候就干掉<br />
反而对于APT之类的攻击WD的表现好到离谱,而APT才是大多数针对性攻击的方法<br />
参照:<br />
https://bbs.kafan.cn/thread-2181276-1-1.html<br />
(需要登陆)<br />
<br />
真正的攻击需要一个攻击链,不是你写出一个exe让目标在电脑上一跑就行了的<br />
如果在钓鱼/漏洞 或者 白利用 或者 真正传输时拦截<br />
那都是防住了

是的，真不行，所以我把windefend关掉，直接裸奔

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355205&amp;ptid=758664" target="_blank"><font color="#999999">龟龟酱 发表于 2020-10-26 18:02</font></a></font><br />
不是windows defender只能玩玩而已<br />
是你的做法是玩玩而已...<br />
WD非常依赖云,而不是启发,所以会在你把这个样 ...</blockquote></div><br />
<br />
我确实对杀毒病毒没什么研究。只是突发奇想想试试手头这几款能不能搞定未知病毒。<br />
<br />
多谢大佬矫正。<img src="static/image/smiley/default/handshake.gif" smilieid="17" border="0" alt="" />

感谢提醒，这就安装360

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355081&amp;ptid=758664" target="_blank"><font color="#999999">大侠饶命 发表于 2020-10-26 17:36</font></a></font><br />
楼主演示有记录吗 没有别的意思 我也想转发一下 好更有说服力 哈哈哈<br />
<br />
顺带问一下 火绒的表现咋样？ ...</blockquote></div><br />
我盆友让我问问&nbsp;&nbsp;火绒的表现咋样？

其他也不行啊<br />
<br />
只要盯上，没啥能行！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

楼主演示有记录吗 没有别的意思 我也想转发一下 好更有说服力 哈哈哈<img src="static/image/smiley/yct/010.gif" smilieid="41" border="0" alt="" /><br />
<br />
顺带问一下 火绒的表现咋样？

在河边玩，迟早的事

你开了云没有？默认没开云查杀

卡巴，最强没有疑问的。用了快十来年了

楼上说的都对<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />。<br />
我不用wd主要是添加个白名单太麻烦了，经常不生效
