# 请问什么是dns解锁奈非呢？？？是中转吗


原理其实是dns劫持

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353237&amp;ptid=758515" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-26 11:36</font></a></font><br />
并不是，资源部分就走你本地的，验证连接走解锁</blockquote></div><br />
所以视频速度还是取决于我的鸡？

<div class="quote"><blockquote><font color="#999999">kkdf 发表于 2020-10-26 12:07</font><br />
<font color="#999999">所以视频速度还是取决于我的鸡？</font></blockquote></div><br />
是的

<i class="pstatus"> 本帖最后由 ymcoming 于 2020-10-26 12:16 编辑 </i><br />
<br />
上面答错了，取决于你的vps和dns解锁服务器，谁弱谁就是瓶颈。<br />
<br />
至于为啥会出现楼主那种奇谈怪论，可能过去netflix是这样的，但现在肯定只会在解锁服务器进行数据传输。<br />
<br />
也就是你的vps自以为访问netflix，实际全部流量转到解锁服务器。奈飞那边也是自认为解锁服务器在看奈飞，根本不知道有第三者。<br />
<br />
做解锁的负担了全部流量的中转。

netflix.com -&gt;解锁用的dns<br />
解锁用的dns -&gt; 解锁机的ip<br />
就是只帮你中转netflix流量到能看netflix的机器

受限制的&nbsp; &nbsp;相当于识别到Netflix的流量就劫持 劫持到自己的dns服务器&nbsp;&nbsp;dns服务器就相当于反代<img id="aimg_e8Za2" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

以后连NF就10M

所谓解锁就是一个代理服务器而已

欢迎找我 5元/月 新加坡/美国奈飞解锁<br />
<br />
实际走的是我服务器的流量 你看多少 我就的用多少<br />
<br />
一群没用过的就在那里胡说<br />
<br />
个个靠吹都是能人 

<i class="pstatus"> 本帖最后由 nat.ee 于 2020-10-26 12:30 编辑 </i><br />
<br />
dns解锁，可以做到，匹配到的绝对域名而走反代，没有在列表内的走正常dns解析，也就是说可以做到奈飞验证部分走dns解锁反代，而视频资源部分走本地。<br />
看来大部分人都是奈飞全走dns解锁反代了<br />
例如a.Netflix.com已添加到列表内，这个域名就走反代并伪造解锁ip返回给终端。<br />
而b.Netflix.com没有添加到列表，就不走反代，实现本地正常解析。<br />
总不会奈飞，网页资源部分和视频资源部分都是同一个绝对域名吧？<br />

