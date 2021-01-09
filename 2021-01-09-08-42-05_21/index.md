# 有三毛的MJJ加速方案都是什么？


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9371186&amp;ptid=759405" target="_blank"><font color="#999999">timotai 发表于 2020-10-29 20:40</font></a></font><br />
我也想一份 cc家的 1H2G60G 带宽1G 请帮一下 多谢了</blockquote></div><br />
平均延迟多少？

杭州BGP -&gt; 上海CN2 -&gt; 日本任意运营商 -&gt; 落地鸡

<i class="pstatus"> 本帖最后由 timotai 于 2020-10-29 21:04 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9371190&amp;ptid=759405" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-29 20:41</font></a></font><br />
平均延迟多少？</blockquote></div><br />
<br />
181

<i class="pstatus"> 本帖最后由 nat.ee 于 2020-10-29 21:27 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9371271&amp;ptid=759405" target="_blank"><font color="#999999">timotai 发表于 2020-10-29 20:53</font></a></font><br />
181</blockquote></div><br />
<div class="blockcode"><div id="code_kcK"><ol><li>acc=&quot;1&quot;<br /><li>advacc=&quot;1&quot;<br /><li>advinacc=&quot;1&quot;<br /><li>wankbps=&quot;1000000&quot;<br /><li>waninkbps=&quot;1000000&quot;<br /><li>maxmode=&quot;1&quot;<br /><li>initialCwndWan=&quot;60&quot;<br /><li>maxCwndWan=&quot;&quot;<br /><li>l2wQLimit=&quot;2048 16384&quot;<br /><li>w2lQLimit=&quot;2048 16384&quot;<br /><li>shaperEnable=&quot;0&quot;<br /><li>smBurstMS=&quot;20&quot;<br /><li>nic_offload=&quot;1&quot;<br /><li>rsc=&quot;1&quot;<br /><li>gso=&quot;1&quot;<br /><li><br /><li>engineNum=&quot;0&quot;<br /><li>shortRttMS=&quot;80&quot;</ol></div><em onclick="copycode($('code_kcK'));">复制代码</em></div><br />
<br />
这里注意下，如果你的锐速 有这个 nic_offload=&quot;1&quot; 参数，你自己测速，改为0或者 1 尝试 测速那个快。就设置那个！<br />
<br />
试试效果是否比BBR好些？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9371441&amp;ptid=759405" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-29 21:23</font></a></font><br />
这里注意下，如果你的锐速 有这个 nic_offload=&quot;1&quot; 参数，你自己测速，改为0或者 1 尝试 测速那个快。 ...</blockquote></div><br />
多谢了 

战略性马克，此贴有大佬出没<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

马克<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img id="aimg_p6Sh1" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

能否科普一下参数啊？我也自己慢慢调调，现在是bbr一把梭哈

马克一下，之前是一键<img id="aimg_WAb36" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366795&amp;ptid=759405" target="_blank"><font color="#999999">Erik 发表于 2020-10-28 23:10</font></a></font><br />
debian10不支持锐速，重装换debian9，现在正在装威兔 ws tls，完了我试试锐速，回头跟你说说感受、</blockquote></div><br />
有效果吗<img id="aimg_Ce8p6" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
