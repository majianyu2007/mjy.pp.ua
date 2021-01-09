# CloudFlare Worker能转发非标准端口吗


<i class="pstatus"> 本帖最后由 dole 于 2020-10-13 12:06 编辑 </i><br />
<br />
如题 想转发非标准端口 如12345等等 nat无法自定义端口 大陆地区访问 求指点<img id="aimg_iOcrU" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

没玩过AWS的CDN，帮顶！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

你试试反带？？

可以

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9293312&amp;ptid=753719" target="_blank"><font color="#999999">llmwxt 发表于 2020-10-13 11:46</font></a></font><br />
没玩过AWS的CDN，帮顶！</blockquote></div><br />
不是aws的那个cf<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img id="aimg_iPUWa" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9293349&amp;ptid=753719" target="_blank"><font color="#999999">dole 发表于 2020-10-13 11:55</font></a></font><br />
不是aws的那个cf</blockquote></div><br />
不好意思，看错了，CF的话，3楼大佬的方法可以试试的！

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9293315&amp;ptid=753719" target="_blank"><font color="#999999">逍遥自在 发表于 2020-10-13 11:47</font></a></font><br />
你试试反带？？</blockquote></div><br />
就是反代 拒绝访问<img src="static/image/smiley/default/mad.gif" smilieid="11" border="0" alt="" /><img id="aimg_h9X26" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 dole 于 2020-10-13 12:05 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9293353&amp;ptid=753719" target="_blank"><font color="#999999">llmwxt 发表于 2020-10-13 11:56</font></a></font><br />
不好意思，看错了，CF的话，3楼大佬的方法可以试试的！</blockquote></div><br />
<br />
无解 Error 526 <br />
Invalid SSL certificate<br />
加http头：Error 1003 <br />
Direct IP access not allowed<img id="aimg_OyPrJ" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9293323&amp;ptid=753719" target="_blank"><font color="#999999">大鸡鸡 发表于 2020-10-13 11:47</font></a></font><br />
可以</blockquote></div><br />
求大佬指点<img src="static/image/smiley/default/loveliness.gif" smilieid="28" border="0" alt="" />

dd<img id="aimg_E45Sh" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
