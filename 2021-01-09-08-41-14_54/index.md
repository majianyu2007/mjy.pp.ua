# 有大佬知道这个怎么排查解决吗


<i class="pstatus"> 本帖最后由 小小白 于 2020-10-24 20:11 编辑 </i><br />
<br />
。。。。。。。

<i class="pstatus"> 本帖最后由 萌墨 于 2020-10-24 20:10 编辑 </i><br />
<br />
把 &amp;nbsp; 去掉就行 会占位的<br />
在body起始的位置那里<br />
<img id="aimg_mCj8x" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://pic.rmb.bdstatic.com/bjh/ce921f822a10602ced221f2fc681d2c5.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<img id="aimg_s244u" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://pic.rmb.bdstatic.com/bjh/9a256dbcc294249c3bb84744a69bd66a.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347347&amp;ptid=758055" target="_blank"><font color="#999999">萌墨 发表于 2020-10-24 20:08</font></a></font><br />
把 &amp;nbsp; 去掉就行 好像会占位的</blockquote></div><br />
是这样&nbsp;&nbsp;但是源码里正常没空格

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347347&amp;ptid=758055" target="_blank"><font color="#999999">萌墨 发表于 2020-10-24 20:08</font></a></font><br />
把 &amp;nbsp; 去掉就行 会占位的<br />
在body起始的位置那里</blockquote></div><br />
<img id="aimg_yuFoC" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://p.pstatp.com/origin/137d000013b020106eaea.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />是这样么，木有空格

<i class="pstatus"> 本帖最后由 sh3dowin 于 2020-10-24 20:42 编辑 </i><br />
<br />
这个文件 wp-content/themes/kratos/assets/css/kratos.min.css?ver=3.2.0<br />
搜 .k-header .banner {<br />
<br />
改为<br />
<br /><div class="blockcode"><div id="code_q1w"><ol><li>.k-header .banner {<br /><li>&nbsp; &nbsp; position: relative;<br /><li>&nbsp; &nbsp; height: 300px;<br /><li>&nbsp; &nbsp; bottom: 28px;<br /><li>}</ol></div><em onclick="copycode($('code_q1w'));">复制代码</em></div>

<i class="pstatus"> 本帖最后由 lllll 于 2020-10-24 20:44 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347412&amp;ptid=758055" target="_blank"><font color="#999999">sh3dowin 发表于 2020-10-24 20:22</font></a></font><br />
这个文件 wp-content/themes/kratos/assets/css/kratos.min.css?ver=3.2.0<br />
<br />
搜 .k-header .banner {</blockquote></div><br />
<br />
这好像是缓存文件&nbsp;&nbsp;强刷就没了&nbsp;&nbsp;<img src="static/image/smiley/default/sweat.gif" smilieid="10" border="0" alt="" />&nbsp;&nbsp;不过我好像知道什么原因了 谢谢大佬<img id="aimg_H40X9" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 sh3dowin 于 2020-10-24 20:44 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347494&amp;ptid=758055" target="_blank"><font color="#999999">lllll 发表于 2020-10-24 20:37</font></a></font><br />
这好像是缓存文件&nbsp;&nbsp;强刷就没了&nbsp; &nbsp; 不过我好像知道什么原因了 谢谢大佬</blockquote></div><br />
<br />
wp-content/themes/kratos/assets/css/kratos.min.css?ver=3.2.0<br />
<br />
这个文件，刚才复制错了，麻烦16#编辑一下把缓存那个url删了，哈哈<br />
<br />
另外好像删了body的那俩个空格最方便

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347510&amp;ptid=758055" target="_blank"><font color="#999999">sh3dowin 发表于 2020-10-24 20:42</font></a></font><br />
wp-content/themes/kratos/assets/css/kratos.min.css?ver=3.2.0<br />
<br />
这个文件，刚才复制错了，麻烦16#编辑 ...</blockquote></div><br />
我刚把缓存插件禁用了&nbsp;&nbsp;是这个&nbsp;&nbsp;谢谢了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img id="aimg_P1zV2" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347412&amp;ptid=758055" target="_blank"><font color="#999999">sh3dowin 发表于 2020-10-24 20:22</font></a></font><br />
这个文件 wp-content/themes/kratos/assets/css/kratos.min.css?ver=3.2.0<br />
搜 .k-header .banner {</blockquote></div><br />
这个也行 加个bottom 增加底部外边距顶上去直接覆盖掉白色那部分<img src="static/image/smiley/yct/010.gif" smilieid="41" border="0" alt="" /><br />
<br />
<img id="aimg_PreR0" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://pic.rmb.bdstatic.com/bjh/c170bcc863c8658a82d2809bfeb4cc7b.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
