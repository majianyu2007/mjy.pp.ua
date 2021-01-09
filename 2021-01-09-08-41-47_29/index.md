# 求助https://files.photo.gallery/ 目录程序怎么不会生成图片缩略图


安装2个扩展已经解决

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273469&amp;ptid=752101" target="_blank"><font color="#999999">西湖老舅 发表于 2020-10-8 21:27</font></a></font><br />
重启php</blockquote></div><br />
卧槽 终于解决问题了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273457&amp;ptid=752101" target="_blank"><font color="#999999">xshell 发表于 2020-10-8 21:24</font></a></font><br />
安装了啊<br />
<br />
图片处理库</blockquote></div><br />
我就知道你了，我这里d.nat.ee 都显示正常。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273506&amp;ptid=752101" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-8 21:33</font></a></font><br />
我就知道你了，我这里d.nat.ee 都显示正常。</blockquote></div><br />
图太多&nbsp;&nbsp;VPS直接跑崩了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273514&amp;ptid=752101" target="_blank"><font color="#999999">xshell 发表于 2020-10-8 21:34</font></a></font><br />
图太多&nbsp;&nbsp;VPS直接跑崩了</blockquote></div><br />
所以，你才需要那个插件，预生成缓存。这样就不崩了。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273506&amp;ptid=752101" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-8 21:33</font></a></font><br />
我就知道你了，我这里d.nat.ee 都显示正常。</blockquote></div><br />
大佬 你知道为什么演示站的缩略图是真实路径：https://files.photo.gallery/demo/_files/cache/images/87249c.240118.1582517278.320.jpg<br />
<br />
而我们的缩略图不是呢？这样不利于cdn缓存啊<br />
这是你的缩略图：http://d.nat.ee/index.php?file=win7%2Fdemo.png&amp;resize=320&amp;567a48.1600753961.139943<br />
这是我的缩略图：https://cf.cdn.xiazai.de/meinv/index.php?file=tp.wcctv.top%2Fassets.baklib.com%2F1f05ee0e-f0ae-4e7b-869d-3422fd3d2bb1%2F00041584448028886.jpg&amp;resize=320&amp;05f14d.1599739024.607431

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273541&amp;ptid=752101" target="_blank"><font color="#999999">xshell 发表于 2020-10-8 21:38</font></a></font><br />
大佬 你知道为什么演示站的缩略图是真实路径：https://files.photo.gallery/demo/_files/cache/images/87 ...</blockquote></div><br />
这个应该和配置文件相关设置的，我没研究。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273549&amp;ptid=752101" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-8 21:40</font></a></font><br />
这个应该和配置文件相关设置的，我没研究。</blockquote></div><br />
研究出来了<br />
image_resize_cache_direct改为true就可以了<br />
这样才利于cdn缓存&nbsp;&nbsp;感谢大佬的解答

我安装了同一家公司的x3 相册程序，也出现无预览图片的情况。相关的插件已经安装，php也重启了，不知道什么原因？一直就是一个圆圈在那里转啊转<img src="static/image/smiley/default/sweat.gif" smilieid="10" border="0" alt="" /><br />
<br />
<img id="aimg_uvdVV" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://www.10086.win/imgs/2020/10/a14f9ed09c7ce9d7.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
