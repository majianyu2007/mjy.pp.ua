# 请教下宝塔面板 怎么使用本地文件安装旧版？


https://www.hostloc.com/thread-747313-1-1.html<br />
<br />
如题<br />
使用上面的历史版文件，在vps上用本地文件安装，安装脚本需要修改那些地方？

我文章已经写了<br /><div class="blockcode"><div id="code_yXa"><ol><li>离线升级步骤：<br /><li>1、下载离线升级包<br /><li>2、将升级包上传到服务器中的/root目录<br /><li>3、解压文件：unzip LinuxPanel-*<br /><li>4、切换到升级包目录： cd panel<br /><li>5、执行升级脚本：bash update.sh<br /><li>6、删除升级包：cd .. &amp;&amp; rm -f LinuxPanel-*.zip &amp;&amp; rm -rf panel</ol></div><em onclick="copycode($('code_yXa'));">复制代码</em></div><br />
<br />
离线升级，也可以离线降级，懂了不

帮顶，不懂！<br />
<br />
等大佬们回答吧！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9385462&amp;ptid=760993" target="_blank"><font color="#999999">cicvc 发表于 2020-11-1 17:40</font></a></font><br />
我文章已经写了</blockquote></div><br />
可以修改安装脚本，安装旧版吗
