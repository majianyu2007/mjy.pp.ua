# 宝塔国际版（aaPanel）会收集哪些信息，附官方解释


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9407998&amp;ptid=762727" target="_blank"><font color="#999999">Easonn 发表于 2020-11-5 18:44</font></a></font><br />
不点同意用户协议，能下一步吗2333</blockquote></div><br />
<br />
这时候就不学习国际通行方法了？<br />
不同意就不进行收集，而不是不给用。

我换oneinstack了，其实都差不多，我现在就缺个文件管理器了

不用它，不用担心这事

用了动不动担心被删库也是麻烦，已经把宝塔拉入黑名单。

唉<br />
不要再用了就好.<br />
还是用LNMP吧.

<i class="pstatus"> 本帖最后由 fullbody 于 2020-11-6 11:01 编辑 </i><br />
<br />
其实当你用浏览器打开宝塔面板的登录页面时，<br />
页面默认会加载宝塔APP的图片，<div class="blockcode"><div id="code_KbB"><ol><li>http://app.bt.cn/static/app.png</ol></div><em onclick="copycode($('code_KbB'));">复制代码</em></div><br />
理论上，就已可以通过浏览器的请求头Referer记录到了用户登录IP，服务器IP，面板端口，安全入口和其他信息，不过这些都在他的网站日志里。<br /><div class="blockcode"><div id="code_U5U"><ol><li>Referer: http://XXX.XXX.XXX.XXX:8888/xsdwdwdd/</ol></div><em onclick="copycode($('code_U5U'));">复制代码</em></div><br />
<br />
国内版国外版都有此情况，打算用aaPanel的注意一下。<br />
可以用浏览器插件伪装Referer和X-Forwarded-For<br />
<br />
注意：ModHeader被爆有安全问题

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9408976&amp;ptid=762727" target="_blank"><font color="#999999">fullbody 发表于 2020-11-5 21:52</font></a></font><br />
其实当你用浏览器打开宝塔面板的登录页面时，<br />
页面默认会加载宝塔APP的图片，<br />
理论上，就已可以通过浏览器 ...</blockquote></div><br />
厉害了...<br />
<br />
但是一下也没能找到合适的替代方案<br />
<br />
主要是小白不懂命令,只会可视化操作<br />
<br />
<img src="static/image/smiley/yct/019.gif" smilieid="49" border="0" alt="" />

收集站点总数不顺带着把站信息也唆一把？

玛德他可怕了，赶紧推荐个国外类似的面板啊

不留后门 怎么甩锅。在天朝没办法 这个必须开后门。不配合出事就找你。所以直接留门甩锅
