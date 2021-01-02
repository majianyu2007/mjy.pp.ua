# 有谁知道宝塔5.9怎么安装1.18版本的nginx吗？


？？？如题<br />
<br />
还有就是contabo美国机器出问题了，一直开不了机！<img id="aimg_S7D9Z" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="76" src="https://i.w3tt.com/images/oNlDM.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" />

手动编译到目录

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403390&amp;ptid=762481" target="_blank"><font color="#999999">iks 发表于 2020-11-4 20:26</font></a></font><br />
手动编译到目录</blockquote></div><br />
搁哪儿？大哥<img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403398&amp;ptid=762481" target="_blank"><font color="#999999">peng123 发表于 2020-11-4 20:28</font></a></font><br />
搁哪儿？大哥</blockquote></div><br />
<br />
/www/server/nginx<br />
<br />
记得改下原目录下的 .pl 里的版本号

手动编译安装，编译目录写宝塔的路径。看我文章《宝塔自定义编译安装 Nginx 并配置 TLS1.3》<br /><div class="blockcode"><div id="code_QDX"><ol><li>https://www.nange.cn/tls13-for-nginx.html</ol></div><em onclick="copycode($('code_QDX'));">复制代码</em></div>

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403617&amp;ptid=762481" target="_blank"><font color="#999999">翠花 发表于 2020-11-4 21:17</font></a></font><br />
手动编译安装，编译目录写宝塔的路径。看我文章《宝塔自定义编译安装 Nginx 并配置 TLS1.3》<br />
 ...</blockquote></div><br />
能在前台显示和配置吗？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403672&amp;ptid=762481" target="_blank"><font color="#999999">peng123 发表于 2020-11-4 21:30</font></a></font><br />
能在前台显示和配置吗？</blockquote></div><br />
必须得可以，我一直都是这么干的。<img src="static/image/smiley/yct/013.gif" smilieid="43" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403672&amp;ptid=762481" target="_blank"><font color="#999999">peng123 发表于 2020-11-4 21:30</font></a></font><br />
能在前台显示和配置吗？</blockquote></div><br />
安装完之后，如果提示更新，就把文件 /www/server/nginx/version.pl和/www/server/nginx/version_check.pl里边的版本号给改成其他的，改成你的名字也是可以的。
