# 阿里云等云服中的1核是物理上的1核还是1线程？


最近又想到了这个问题，<br />
<br />
暂且不讨论那些共享计算的机器~<br />
<br />
如果是1线程的话，那么一个物理核上的隔壁满载了是不是有影响。<br />
<br />
如果是1核的话，能卖的机器是不是就少了一些？

阿里云的是线程，oralce的那才是1核<br />
当然不排除阿里云母鸡500核500线程

一直以为是1核心1线程。等楼下真理<img id="aimg_oQEmE" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

刚刚看了一下阿里云的非共享实列，最低都是2核起卖……<br />
如果是线程的话。是不是代表只能享受到实际一个核心满载？

肯定是1核啊<br />


你这就跟问女人爽不爽一个道理。人家都说了很爽了就行了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9358223&amp;ptid=758910" target="_blank"><font color="#999999">tir 发表于 2020-10-27 11:45</font></a></font><br />
肯定是1核啊</blockquote></div><br />
咋感觉不太像1核的情况……

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9358249&amp;ptid=758910" target="_blank"><font color="#999999">ABCHINA 发表于 2020-10-27 11:50</font></a></font><br />
阿里云的是线程，oralce的那才是1核<br />
当然不排除阿里云母鸡500核500线程</blockquote></div><br />
阿里云应该是线程吧……8269CY是26核52线。双路的话是104，4路的话是208 和阿里云上的销售页面可以对上。<br />
<br />
猜测母机就是208核.＞3072G内存这样吧……（可选的最高配置）

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9358287&amp;ptid=758910" target="_blank"><font color="#999999">guoguomiao 发表于 2020-10-27 11:57</font></a></font><br />
阿里云应该是线程吧……8269CY是26核52线。双路的话是104，4路的话是208 和阿里云上的销售页面可以对上。 ...</blockquote></div><br />
<br />
目前的商家，除了oracle，其他商家没见过按真实核卖过，都是线程

一分钱一分货 要真核就买毒妇
