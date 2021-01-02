# 关于堡塔公司协助安全调查


<i class="pstatus"> 本帖最后由 dmking923 于 2020-11-4 20:36 编辑 </i><br />
<br />
<font size="4">看到堡塔公司协助调查的帖子，吓得赶紧把国外小鸡上的宝塔的账号关联取消了<br />
<br />
国内的取消不掉，于是重装机，换IP，可是一下习惯性手贱，又装上宝塔了，但这无意中让我发现一个“漏洞”，装完宝塔后进入会强制要求绑定账户，这个时候重置一下面板，关闭强制验证，再进去就不会提示绑账号了<br />
<br />
虽然说不敢违法乱纪的大事，但是也存了10来个T的国产大姐姐（不喜欢国外的），还都没重复，都是辛辛苦苦筛选出来的。还是凡事小心为妙！</font>

兄弟，借一部说话

sed -i &quot;s|if (bind_user == 'True') {|if (bind_user == 'REMOVED') {|g&quot; /www/server/panel/BTPanel/static/js/index.js

求个url

怎么重置面板

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403451&amp;ptid=762488" target="_blank"><font color="#999999">云生 发表于 2020-11-4 20:39</font></a></font><br />
怎么重置面板</blockquote></div><br />
ssh<br />
bt<img id="aimg_cweIP" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

兄弟，借一部说话

所有国产的闭源软件都不能相信，国产的开源软件口碑好的可以相信。

<i class="pstatus"> 本帖最后由 zaeve 于 2020-11-4 21:17 编辑 </i><br />
<br />
什么鬼？为什么说的那么复杂？<br />
新装面板要登陆宝塔账号的，直接用ublock把那个登陆窗口临时屏蔽掉不就好了！？<br />
只要登陆面板(不是宝塔账号)一次，就再也不会要你登陆宝塔账号了。<br />
还要什么重置？？？<img id="aimg_e4RQQ" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
