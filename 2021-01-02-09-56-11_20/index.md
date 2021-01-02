# 现在宝塔不能反代google了吗


<i class="pstatus"> 本帖最后由 FXB 于 2020-11-5 20:43 编辑 </i><br />
<br />
<br />
<img id="aimg_PJht3" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="386" src="http://www.s3tu.com/images/2020/11/05/imagebbd6f.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<br />
<br />

<ignore_js_op>

<img id="aimg_141043" aid="141043" src="static/image/common/none.gif" zoomfile="forum.php?mod=attachment&aid=MTQxMDQzfGEyODk4MmNkfDE2MDk1Mzg4Njh8NDczNDR8NzYyODA2&noupdate=yes&nothumb=yes" file="forum.php?mod=attachment&aid=MTQxMDQzfGEyODk4MmNkfDE2MDk1Mzg4Njh8NDczNDR8NzYyODA2&noupdate=yes" class="zoom" onclick="zoom(this, this.src, 0, 0, 0)" width="400" id="aimg_141043" inpost="1" onmouseover="showMenu({'ctrlid':this.id,'pos':'12'})" />

<div class="tip tip_4 aimg_tip" id="aimg_141043_menu" style="position: absolute; display: none" disautofocus="true">
<div class="xs0">
<p><strong>QQ图片20201105145854.png</strong> <em class="xg1">(25.54 KB, 下载次数: 0)</em></p>
<p>
<a href="forum.php?mod=attachment&amp;aid=MTQxMDQzfGEyODk4MmNkfDE2MDk1Mzg4Njh8NDczNDR8NzYyODA2&amp;nothumb=yes" target="_blank">下载附件</a>

</p>

<p class="xg1 y">2020-11-5 14:59 上传</p>

</div>
<div class="tip_horn"></div>
</div>

</ignore_js_op>
<br />
<br />
<br />
<br />
好像是没办法用了哇<br />
<br />
<br />
<strong><font size="6">已经解决</font></strong><br />
<br />
宝塔版本的问题...新版BUG 这么久居然不修复<br />
<br />
<br />
<img id="aimg_ovmDO" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="228" src="http://www.s3tu.com/images/2020/11/05/image6024a.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<br />
<br />
<strong><font color="Red">在7.4.5以前的版本可以正常使用，但在7.45版本以后，反向代理“发送域名”字段无法保存，只能手动改配置文件</font></strong>

活久见<img id="aimg_AVvNM" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9406792&amp;ptid=762806" target="_blank"><font color="#999999">hellfires 发表于 2020-11-5 15:10</font></a></font><br />
你就不会填下发送域名吗？</blockquote></div><br />
填了之后 点击保存就自动这样了

本地开启ssl了吗？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9406858&amp;ptid=762806" target="_blank"><font color="#999999">百度网盘 发表于 2020-11-5 15:22</font></a></font><br />
本地开启ssl了吗？</blockquote></div><br />
开了的&nbsp;&nbsp;代loc的论坛都没问题...

目标URL<br />
https://www.google.com<br />
发送域名<br />
www.google.com<br />
<br />
不行的话。我把宝塔收购了！我自用怎么旧。没试过不行

<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

加个内容替换？<img id="aimg_duWbx" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

谷歌服务器监听楼主域名并返回谷歌搜索数据
