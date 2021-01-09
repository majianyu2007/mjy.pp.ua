# 有三毛的MJJ加速方案都是什么？


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9364359&amp;ptid=759405" target="_blank"><font color="#999999">Erik 发表于 2020-10-28 15:37</font></a></font><br />
大佬，我是debian9，本地北方联通，到三毛一般ping在130ms-180ms，求参数，<br />
<br />
多谢了 ...</blockquote></div><br />
你到这里测ping http://ping.chinaz.com/ 取消海外，然后测完看平均值，还有你的是多少内存，CPU是1核还是其他？ 这些告诉我就行<br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366439&amp;ptid=759405" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-28 21:40</font></a></font><br />
你到这里测ping http://ping.chinaz.com/ 取消海外，然后测完看平均值，还有你的是多少内存，CPU是1核还 ...</blockquote></div><br />
多谢大佬，<br />
<br />
我的三毛机内存是419M<br />
我又开了1G多的Swap<br />
<br />
现在晚高峰到国内平均延迟250ms

<i class="pstatus"> 本帖最后由 nat.ee 于 2020-10-28 22:17 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366552&amp;ptid=759405" target="_blank"><font color="#999999">Erik 发表于 2020-10-28 22:07</font></a></font><br />
多谢大佬，<br />
<br />
我的三毛机内存是419M</blockquote></div><br />
<div class="blockcode"><div id="code_I7p"><ol><li>acc=&quot;1&quot;<br /><li>advacc=&quot;1&quot;<br /><li>advinacc=&quot;1&quot;<br /><li>wankbps=&quot;1000000&quot;<br /><li>waninkbps=&quot;1000000&quot;<br /><li>maxmode=&quot;1&quot;<br /><li>initialCwndWan=&quot;80&quot;<br /><li>l2wQLimit=&quot;419 3352&quot;<br /><li>w2lQLimit=&quot;419 3352&quot;<br /><li>shaperEnable=&quot;0&quot;<br /><li>smBurstMS=&quot;27&quot;<br /><li>nic_offload=&quot;1&quot;<br /><li>rsc=&quot;1&quot;<br /><li>gso=&quot;1&quot;<br /><li><br /><li>shortRttMS=&quot;130&quot;</ol></div><em onclick="copycode($('code_I7p'));">复制代码</em></div><br />
<br />
这里注意下，如果你的锐速 有这个 nic_offload=&quot;1&quot; 参数，你自己测速，改为0或者 1 尝试 测速那个快。就设置那个！<br />
<br />
试试效果是否比BBR好些？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366595&amp;ptid=759405" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-28 22:14</font></a></font><br />
这里注意下，如果你的锐速 有这个 nic_offload=&quot;1&quot; 参数，你自己测速，改为0或者 1 尝试 测速那个快。 ...</blockquote></div><br />
好的，多谢大佬

效果怎么样，楼主试出来没

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366646&amp;ptid=759405" target="_blank"><font color="#999999">Erik 发表于 2020-10-28 22:31</font></a></font><br />
好的，多谢大佬</blockquote></div><br />
老哥试了效果咋样呢？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366783&amp;ptid=759405" target="_blank"><font color="#999999">coderzgh 发表于 2020-10-28 23:07</font></a></font><br />
老哥试了效果咋样呢？</blockquote></div><br />
<br />
debian10不支持锐速，重装换debian9，现在正在装威兔 ws tls，完了我试试锐速，回头跟你说说感受、<br />
<br />
<br />
三毛晚高峰太卡，石头盘

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366795&amp;ptid=759405" target="_blank"><font color="#999999">Erik 发表于 2020-10-28 23:10</font></a></font><br />
debian10不支持锐速，重装换debian9，现在正在装威兔 ws tls，完了我试试锐速，回头跟你说说感受、</blockquote></div><br />
我用BBR魔改内核+暴力BBR魔改加速 效果还行把 锐速没试验

这么多讲究么！我都是一键！

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9364063&amp;ptid=759405" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-28 14:44</font></a></font><br />
锐速绝对秒bbr<br />
我可以根据你的配置和延迟给你配一份锐速自定义参数。</blockquote></div><br />
我也想一份 cc家的 1H2G60G 带宽1G 请帮一下 多谢了
