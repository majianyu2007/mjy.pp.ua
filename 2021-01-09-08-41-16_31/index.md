# 想把有图比上面一个UP主的所有视频下载下来，用什么软件？


批量下载的，求推荐，谢谢大佬

有图比 -dl刚被禁止

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9348926&amp;ptid=758198" target="_blank"><font color="#999999">绿豆 发表于 2020-10-25 10:28</font></a></font><br />
有图比 -dl刚被禁止</blockquote></div><br />
是吗？什么时候的事儿啊

downie

<img src="static/image/smiley/default/sweat.gif" smilieid="10" border="0" alt="" />有图比客户端真tm多的广告，不是一般的多 

<div class="quote"><blockquote><font color="#999999">绿豆 发表于 2020-10-25 10:28</font><br />
<font color="#999999">有图比 -dl刚被禁止</font></blockquote></div><br />
Github而已，Gitee继续『CNNB抗投诉』

付费的有

替换一下 ${uploader}<br />
<br /><div class="blockcode"><div id="code_F5z"><ol><li>&nbsp; &nbsp; &nbsp; &nbsp; docker run \<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; --rm \<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; --name 有图比-dl \<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; --mount type=bind,src=/etc/localtime,dst=/etc/localtime,readonly \<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; --mount type=bind,src=/mediadata/jellyfin/media/有图比/,dst=/output/ \<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; newnius/有图比-dl \<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; 有图比-dl \<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; --ignore-errors \<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; --proxy 'http://192.168.1.2:8118' \<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; -o '/output/%(upload_date)s/%(uploader)s_%(id)s.%(ext)s' \<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;https://www.有图比.com/playlist?list=${uploader}&quot;</ol></div><em onclick="copycode($('code_F5z'));">复制代码</em></div><br />
<br />
有图比 换成 you*tube

4k video downloader
