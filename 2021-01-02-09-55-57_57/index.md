# HZ的4TX2机器，安装问题


<i class="pstatus"> 本帖最后由 ABCHINA 于 2020-11-4 19:50 编辑 </i><br />
<br />
看着楼上一堆装逼回复的<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /> <br />
自己没试过就来发<br />
<br />
<br />
分区的时候创建一个1MiB的biosboot分区<br />
<br /><div class="blockcode"><div id="code_C8t"><ol><li>说明<br /><li>基于BIOS的系统需要一个特殊的分区才能从GPT磁盘标签引导。要继续，请创建一个1MiB“biosboot”类型的分区<br /><li><br /><li>通常出现此问题的服务器的硬件中单块硬盘的大小超过2TB<br /><li>(MBR,GPT分区表问题导致)</ol></div><em onclick="copycode($('code_C8t'));">复制代码</em></div>
