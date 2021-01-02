# 申请ssl报错怎么解决啊，dns是华为云的


<i class="pstatus"> 本帖最后由 baijia7758 于 2020-10-24 14:26 编辑 </i><br />
<br />
Verify error<img src="static/image/smiley/default/biggrin.gif" smilieid="3" border="0" alt="" />NS problem: SERVFAIL looking up A for sg.v2***.xxx.cn - the domain's nameservers may be malfunctioning<br />
[Sat 24 Oct 2020 02:07:48 PM CST] Please add '--debug' or '--log' to check more details.<br />
[Sat 24 Oct 2020 02:07:48 PM CST] See: https://github.com/acmesh-official/acme.sh/wiki/How-to-debug-acme.sh<br />
这个要怎么解决，有大佬知道吗？

你号没了

换别的DNS，这bug都存在N久了

1. 请把 v2*** 打上星号；<br />
2. 华为云DNS有bug，建议更换NS<img id="aimg_Jv805" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9345794&amp;ptid=757960" target="_blank"><font color="#999999">iks 发表于 2020-10-24 14:21</font></a></font><br />
1. 请把 v2*** 打上星号；<br />
2. 华为云DNS有bug，建议更换NS</blockquote></div><br />
我换dnspod了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9345832&amp;ptid=757960" target="_blank"><font color="#999999">baijia7758 发表于 2020-10-24 14:27</font></a></font><br />
我换dnspod了</blockquote></div><br />
迁移记录后等NS生效就行了（最长需要48小时，最短数分钟）<img id="aimg_OXLmX" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

换DNS 再切回来&nbsp;&nbsp;很多人都遇到了
