# 手持绿云东京的，机器有被从本地登录重启丢数据吗


<i class="pstatus"> 本帖最后由 ABCHINA 于 2020-11-4 13:58 编辑 </i><br />
<br />
24刀的，刚发现网站连不上了，<br />
uptime<br />
13:40:27 up&nbsp;&nbsp;2:09<br />
我想看看为何重启，发现 /var/log/被清空了，一个日志文件都没了。。<br />
我又发现ssh登录了<br />
2020-11-04 11:32:25&nbsp; &nbsp; &nbsp; &nbsp; 本地登录&nbsp; &nbsp; &nbsp; &nbsp; adm&nbsp; &nbsp; &nbsp; &nbsp; tty1<br />
2020-11-04 11:28:38&nbsp; &nbsp; &nbsp; &nbsp; 本地登录&nbsp; &nbsp; &nbsp; &nbsp; adm&nbsp; &nbsp; &nbsp; &nbsp; tty1<br />
你没看错，是本地登录，也就是VNC，谁有VNC权限呢，除了本人和 商家，没有别人有了吧<img src="static/image/smiley/yct/014.gif" smilieid="45" border="0" alt="" /> <br />
<br />
极其恐怖啊

而且 <br />
&nbsp; &nbsp; &nbsp; &nbsp; adm&nbsp; &nbsp; &nbsp; &nbsp; adm&nbsp; &nbsp; &nbsp; &nbsp; /var/adm&nbsp; &nbsp; &nbsp; &nbsp; /bin/bash&nbsp; &nbsp; &nbsp; &nbsp; adm<br />
adm默认权限应该是&nbsp; &nbsp; &nbsp; &nbsp; adm&nbsp; &nbsp; &nbsp; &nbsp; adm&nbsp; &nbsp; &nbsp; &nbsp; /var/adm&nbsp; &nbsp; &nbsp; &nbsp; /sbin/nologin （禁止登录）&nbsp; &nbsp; &nbsp; &nbsp; adm<br />
为何 自己ISO安装的系统，绿云都会去篡改你的数据呢？

哈哈哈

不懂<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" /><br />
这个你得工单问问

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9401450&amp;ptid=762312" target="_blank"><font color="#999999">茎肛互撸娃 发表于 2020-11-4 13:59</font></a></font><br />
不懂<br />
这个你得工单问问</blockquote></div><br />
很明显这不是被入侵，而是从救援模式设置了adm密码，然后从本地登录，操作了一系列之后，删除了系统中所有的日志

绿云也许是在你VPS查找有没有它感兴趣的DJJ.

绿云机器在xtom，中国人的，不可信

卧槽，我也是 不过我流量被清0的 怀疑后台问题 商家不认 我流量自己算才用了100 2今天一看1t就没了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9402247&amp;ptid=762312" target="_blank"><font color="#999999">xilal 发表于 2020-11-4 16:16</font></a></font><br />
卧槽，我也是 不过我流量被清0的 怀疑后台问题 商家不认 我流量自己算才用了100 2今天一看1t就没了 ...</blockquote></div><br />
发工单了 一样不认，我怀疑 他家的后台被入侵了


<ignore_js_op>

<img id="aimg_141015" aid="141015" src="static/image/common/none.gif" zoomfile="forum.php?mod=attachment&aid=MTQxMDE1fDNlODJiMWU0fDE2MDk1MzE0NTB8NDczNDR8NzYyMzEy&noupdate=yes&nothumb=yes" file="forum.php?mod=attachment&aid=MTQxMDE1fDNlODJiMWU0fDE2MDk1MzE0NTB8NDczNDR8NzYyMzEy&noupdate=yes" class="zoom" onclick="zoom(this, this.src, 0, 0, 0)" width="135" id="aimg_141015" inpost="1" onmouseover="showMenu({'ctrlid':this.id,'pos':'12'})" />

<div class="tip tip_4 aimg_tip" id="aimg_141015_menu" style="position: absolute; display: none" disautofocus="true">
<div class="xs0">
<p><strong>Screenshot_2020-11-04-13-19-26-137_com.android.chrome.jpg</strong> <em class="xg1">(8.83 KB, 下载次数: 0)</em></p>
<p>
<a href="forum.php?mod=attachment&amp;aid=MTQxMDE1fDNlODJiMWU0fDE2MDk1MzE0NTB8NDczNDR8NzYyMzEy&amp;nothumb=yes" target="_blank">下载附件</a>

</p>

<p class="xg1 y">2020-11-4 16:28 上传</p>

</div>
<div class="tip_horn"></div>
</div>

</ignore_js_op>
&nbsp;&nbsp;给你看下这是我看到的登录页面 还有商家说 重置带宽从现在起两天，你需要自己检查使用情况 意思就是我流量，这个月我可以重新用呢吗 
