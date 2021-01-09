# 备份数据都用的啥方案


目前家里树莓派+一个良心云轻量，凌晨自动读取数据库所有表数据，重新插入一下。自己写代码，还有什么现成的方案么。

直接连GD，宝塔每天自动备份导入！<br />
<br />
当然这不是我的主意，是帮我做站的大佬！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9385670&amp;ptid=761009" target="_blank"><font color="#999999">llmwxt 发表于 2020-11-1 18:30</font></a></font><br />
直接连GD，宝塔每天自动备份导入！<br />
<br />
当然这不是我的主意，是帮我做站的大佬！</blockquote></div><br />
不会宝塔，基本都是自己开发。

宝塔定时任务

我都是宝塔自动备份到谷歌云盘

除了宝塔没别的了么。。。

borgbackup 

rclone每天自动上传指定目录就行了。

rsync 定时同步备份 
