# c#  为什么不能直接设置cookie


明明都可以直接设置headers了，为什么cookie还要弄成字典形式呢&nbsp;&nbsp;字符串不香吗

帮顶，技术大佬回答吧！<br />
<br />
我就只能看看答案了！<br />
<br />
<img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /><img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /><img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" />

<i class="pstatus"> 本帖最后由 h20 于 2020-10-24 22:18 编辑 </i><br />
<br />
可以啊，怎么不可以，cookiecontaner<br />
<br />
OO的一个设计原则就是高内聚，低耦合，要封装成对象<br />
<br />
你还是适合去用python<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" /> 

建议用HttpHelp这个库<br />
http://httphelper.sufeinet.com/

可算可见个同行了。net core 后用HttpClient，以前HttpWebRequest

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9348151&amp;ptid=758119" target="_blank"><font color="#999999">斌斌 发表于 2020-10-24 22:59</font></a></font><br />
可算可见个同行了。net core 后用HttpClient，以前HttpWebRequest</blockquote></div><br />
HttpWebRequest 真难用 我快学吐了&nbsp;&nbsp;python 的requests真是优雅

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9348017&amp;ptid=758119" target="_blank"><font color="#999999">Rom 发表于 2020-10-24 22:26</font></a></font><br />
建议用HttpHelp这个库<br />
http://httphelper.sufeinet.com/</blockquote></div><br />
399&nbsp;&nbsp;劝退了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9348217&amp;ptid=758119" target="_blank"><font color="#999999">wop 发表于 2020-10-24 23:26</font></a></font><br />
HttpWebRequest 真难用 我快学吐了&nbsp;&nbsp;python 的requests真是优雅</blockquote></div><br />
HttpWebRequest 都是淘汰的了。HttpClient了。语言这东西真不好劝。感觉还是vs2019+C# 舒服

没有实现不了的功能，只有懒得动手的码农。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9348218&amp;ptid=758119" target="_blank"><font color="#999999">wop 发表于 2020-10-24 23:27</font></a></font><br />
399&nbsp;&nbsp;劝退了</blockquote></div><br />
库免费 源码收费 下载DLL引用就完了
