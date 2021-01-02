# 听说racknerd跑完流量会清退么


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9450670&amp;ptid=766286" target="_blank"><font color="#999999">开腥小站长 发表于 2020-11-13 21:51</font></a></font><br />
都是狠人……</blockquote></div><br />
太含蓄了，自信点，都是垃圾

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9449607&amp;ptid=766286" target="_blank"><font color="#999999">private 发表于 2020-11-13 17:55</font></a></font><br />
我一个朋友想让我问一下， 怎么瞬间跑完</blockquote></div><br />
<br />
有VPS流量消耗脚本，RN是计算下行流量，于是我就写了个疯狂GET的脚本<br />
【消耗VPS流量工具】<br />
新建一个run.sh脚本，将下面的代码复制到run.sh文件里<br />
#!/bin/bash<br />
echo 将开消耗您的流量，此脚本占用宽带。<br />
echo 将与8秒后开始运行<br />
sleep 8<br />
echo 正在检测环境<br />
yum install screen -y<br />
echo starting...<br />
echo 若要停止,重启服务器即可<br />
sleep 3<br />
screen_name=$&quot;run&quot;&nbsp;&nbsp;<br />
screen -dmS $screen_name&nbsp;&nbsp;<br />
cmd=$&quot;while true ;do wget -O /dev/null https://ftp.ncbi.nih.gov/50GB; done;&quot;;&nbsp;&nbsp;<br />
screen -x -S $screen_name -p 0 -X stuff &quot;$cmd&quot;&nbsp;&nbsp;<br />
screen -x -S $screen_name -p 0 -X stuff $'\n'&nbsp;&nbsp;<br />
echo&nbsp;&nbsp;请时刻留意此脚本更新<br />
<br />
使用方法<br />
chmod +x run.sh<br />
bash run.sh
