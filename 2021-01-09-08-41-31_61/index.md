# RIAA请求GitHub删除有图比DL代码引争议


<i class="pstatus"> 本帖最后由 fule 于 2020-10-27 00:13 编辑 </i><br />
<br />
近日，已归为微软旗下的 GitHub 响应美国唱片业协会 RIAA 的 DMCA 删除请求，删除了一个开源的 有图比 视频下载命令行应用工具 有图比-DL 的代码，引发了开源界的争议。<br />
<img id="aimg_lep2e" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://kyun.ltyuanfang.cn/tc/2020/10/26/35080a8e2a69c.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
根据美国法律专业人士的说法，该工具违反了美国版权法第 1201 条，因为它的明确用意是“规避 有图比 等授权流服务使用的技术保护措施”，并未经 RIAA 授权“复制和分发这些视频“。<br />
<br />
而 有图比-DL 的支持者则认为该工具具有合理合法的用途，包括从 有图比 下载用户自己发布的内容或备份可能由于其他原因而被删除的视频。 <br />
<br />
”有图比-DL 是用于格式转换的极其强大且有用的工具，它在档案管理员中非常受欢迎，并且拥有广泛的合理用途。RIAA 的立场太过激进。“<br />
<br />
” 有图比-DL 是具有合法用途的合法工具。RIAA 要求将其从 Github 中删除的举动是令人失望的，最终可能会适得其反。”<br />
<br />
这次事件很容易让人们回想起 1990 年代开放源代码尚未流行的日子，当时的 RIAA 也进行了一场反开源的战斗，他们试图阻止 DeCSS（DVD 编解码器的解密代码）在互联网上传播。最终，当时的黑客们以把 DeCss 代码打印在 T 恤上的形式进行抗争，并通过后续一系列的努力成功让美国版权法认可了开源软件的存在。<br />
目前，微软还没有对此事发表任何官方评论，只是说代码的维护者有权提出上诉，如果上诉成功则可以恢复其代码。

建议把RIAA负责人的diao剁了，因为他有犯罪的工具

还有这种事,揍他狗日的.&nbsp;&nbsp;神马? DMCA ,那没事了! 惹不起惹不起

电脑可以下载侵权电影应该禁止使用

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9356868&amp;ptid=758793" target="_blank"><font color="#999999">TITAN-LOC 发表于 2020-10-27 00:00</font></a></font><br />
建议把RIAA负责人的diao剁了，因为他有犯罪的工具</blockquote></div><br />
<img src="static/image/smiley/yct/011.gif" smilieid="33" border="0" alt="" />赞同

由于各种原因，GitHub 用户可以从任何一个 repo 的 remote 通过类似 git fetch origin [COMMIT-HASH] 的方式获取其 fork 树上的任何一个 repo 的 commit。也就是说，在 fork repo 中提交的内容可以通过在原 repo 的 remote 上进行 fetch 来获取。又由于用户不能删除 PR，一旦内容被以 PR 的形式提交，PR 中的 commit 就会一直保留。通过这样的方法，用户 Stephen304 将一份 10 月 23 日的 有图比-dl 源码树放在了 github/dmca 上。<br />
<br />
用户可以通过以下方式获取这段源码树：<br />
git clone https://github.com/github/dmca.git &amp;&amp; cd dmca<br />
git fetch origin 416da574ec0df3388f652e44f7fe71b1e3a4701f<br />
git checkout 416da574ec0df3388f652e44f7fe71b1e3a4701f<br />
<br />
src: https://news.ycombinator.com/item?id=24882921<br />
seealso: https://github.com/github/dmca/pull/8142<br />
seealso: https://github.com/github/dmca/tree/416da574ec0df3388f652e44f7fe71b1e3a4701f<img id="aimg_HlWxs" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9356914&amp;ptid=758793" target="_blank"><font color="#999999">wqz 发表于 2020-10-27 00:20</font></a></font><br />
由于各种原因，GitHub 用户可以从任何一个 repo 的 remote 通过类似 git fetch origin [COMMIT-HASH] 的方 ...</blockquote></div><br />
<br />
哈哈,这个好&nbsp; &nbsp; &nbsp; &nbsp; <br />


卧槽，这么好的工具。

google请求的话还能理解，youtu-be又不是他家的
