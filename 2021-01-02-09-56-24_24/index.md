# 全球WordPress技术论坛


WordPress怎么设置不调用二级栏目？<br />
<br />
<br />
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &lt;?php wp_nav_menu( array( 'theme_location' =&gt; 'top-menu', 'menu_class' =&gt; 'top-menu', 'fallback_cb' =&gt; 'default_menu' ) ); ?&gt;<br />
<br />
这样写二级栏目也调用出来,跑到导航上来了<br />
<br />
<br />
<br />
<img id="aimg_YaOFq" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/11/14/XhUgqPzai8vBIVA.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

外观-菜单里调吧，想搞成下拉菜单需要js或者样式配合。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9452199&amp;ptid=766527" target="_blank"><font color="#999999">胖虎 发表于 2020-11-14 10:50</font></a></font><br />
外观-菜单里调吧，想搞成下拉菜单需要js或者样式配合。</blockquote></div><br />
下拉菜单已经有了，这是top顶部调用不是菜单，centos哪个是调出来的二级栏目已经占用了导航的位置，怎么只调用一级栏目不调用二级栏目

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9452199&amp;ptid=766527" target="_blank"><font color="#999999">胖虎 发表于 2020-11-14 10:50</font></a></font><br />
外观-菜单里调吧，想搞成下拉菜单需要js或者样式配合。</blockquote></div><br />
我知道了。大佬，谢谢，重建个菜单就可以了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />
