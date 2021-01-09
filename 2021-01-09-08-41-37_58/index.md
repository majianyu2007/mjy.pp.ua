# HZ杜甫DD一天了没成来个大佬拯救一下吧？


<i class="pstatus"> 本帖最后由 gvf 于 2020-10-26 19:46 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355668&amp;ptid=758699" target="_blank"><font color="#999999">evils 发表于 2020-10-26 19:43</font></a></font><br />
不会&nbsp;&nbsp;刚接手 只会重装</blockquote></div><br />
<br />
https://www.liujason.com/article/371.html<br />
按照上面的关闭raid，你的应该没有硬raid卡，更改完no raid重装完然后再dd

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355658&amp;ptid=758699" target="_blank"><font color="#999999">evils 发表于 2020-10-26 19:41</font></a></font></blockquote></div><br />
这配置的应该没啥坑。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355673&amp;ptid=758699" target="_blank"><font color="#999999">gvf 发表于 2020-10-26 19:44</font></a></font><br />
https://www.liujason.com/article/371.html<br />
按照上面的关闭raid，你的应该没有硬raid卡，更改完no raid ...</blockquote></div><br />
然后这个命令吗？<br /><div class="blockcode"><div id="code_qV8"><ol><li>wget -qO- http://d.nat.ee/win10/win10-ltsc-x64-cn.vhd.gz |gunzip -dc |dd of=/dev/vda</ol></div><em onclick="copycode($('code_qV8'));">复制代码</em></div>

<i class="pstatus"> 本帖最后由 gvf 于 2020-10-26 19:50 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355683&amp;ptid=758699" target="_blank"><font color="#999999">evils 发表于 2020-10-26 19:46</font></a></font><br />
然后这个命令吗？</blockquote></div><br />
<br />
wget -O- &quot;http://d.nat.ee/win10/win10-ltsc-x64-cn.vhd.gz&quot; | gunzip | dd of=/dev/sda<br />
详细的话看秋水博客<br />
https://teddysun.com/545.html

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355688&amp;ptid=758699" target="_blank"><font color="#999999">gvf 发表于 2020-10-26 19:47</font></a></font><br />
wget -O- &quot;http://d.nat.ee/win10/win10-ltsc-x64-cn.vhd.gz&quot; | gunzip | dd of=/dev/sda<br />
详细的话看秋水 ...</blockquote></div><br />
wget -O- &quot;DD download URL&quot; | gunzip | dd of=/dev/sda<br />
<br />
这个呀？

<i class="pstatus"> 本帖最后由 StudyOverseas 于 2020-10-26 19:53 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355683&amp;ptid=758699" target="_blank"><font color="#999999">evils 发表于 2020-10-26 19:46</font></a></font><br />
然后这个命令吗？</blockquote></div><br />
<br />
Hetzner的话DD没问题啊<br />
https://www.liujason.com/article/818.html<br />
<br />
要注意磁盘的盘符，博客里有写<br /><div class="quote"><blockquote>这里一定要注意，因为HZ是按磁盘顺序进行启动引导的，所以最好把其他盘都给删掉分区并且抹除（fdisk /dev/sd{a,b,c}）。另外有nvme盘的话，dd的路径要改成对应的nvme盘符</blockquote></div>

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355692&amp;ptid=758699" target="_blank"><font color="#999999">evils 发表于 2020-10-26 19:51</font></a></font><br />
wget -O- &quot;DD download URL&quot; | gunzip | dd of=/dev/sda<br />
<br />
这个呀？</blockquote></div><br />
对，zsbd

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355694&amp;ptid=758699" target="_blank"><font color="#999999">gvf 发表于 2020-10-26 19:52</font></a></font><br />
对，zsbd</blockquote></div><br />
<img src="static/image/smiley/default/loveliness.gif" smilieid="28" border="0" alt="" /> 然后用我刚才那个安装包可以嘛

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355697&amp;ptid=758699" target="_blank"><font color="#999999">evils 发表于 2020-10-26 19:53</font></a></font><br />
然后用我刚才那个安装包可以嘛</blockquote></div><br />
对的，换成安装包的url，dd命令，重启之后等几分钟就可以连上了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9355706&amp;ptid=758699" target="_blank"><font color="#999999">gvf 发表于 2020-10-26 19:54</font></a></font><br />
对的，换成安装包的url，dd命令，重启之后等几分钟就可以连上了</blockquote></div><br />
原来 no raid 是关键。。。
