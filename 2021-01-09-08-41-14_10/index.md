# rclone sync和COPY有什么区别呢


看了下这两个命令都可以同步本地文件到远程<br />
这两个命令会不会删除本地的文件？<br />
备份的话哪个比较的好，用完sync可以再用 copy 同步一次吗？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9346777&amp;ptid=758017" target="_blank"><font color="#999999">corta 发表于 2020-10-24 17:51</font></a></font><br />
cpoy sync都 不是 按大小/修改时间/MD5 判断文件的，盲猜按是文件名，备份的话要找别的支持历史版本的玩意 ...</blockquote></div><br />
<div class="quote"><blockquote>rclone copy<br />
Copy files from source to dest, skipping already copied.<br />
Synopsis<br />
Copy the source to the destination. Doesn't transfer unchanged files, testing by size and modification time or MD5SUM. Doesn't delete files from the destination.<br />
https://rclone.org/commands/rclone_copy/</blockquote></div><br />
<div class="quote"><blockquote>rclone sync<br />
Make source and dest identical, modifying destination only.<br />
Synopsis<br />
Sync the source to the destination, changing the destination only. Doesn't transfer unchanged files, testing by size and modification time or MD5SUM. Destination is updated to match source, including deleting files if necessary.<br />
https://rclone.org/commands/rclone_sync/</blockquote></div><br />
<br />
建议多看看官方文档

mark一下，同问，一会过来看看

A copy B&nbsp;&nbsp;发现B中没有的A中有的文件，从A复制到B<br />
A sync B&nbsp;&nbsp;找出AB中不同的文件，B有的A没有的删，A有的B没有的复制，完成后B中的文件和A中的一致

一个是增量同步，一个是整个复制

区别就是会不会删除远程的文件

cpoy sync都 不是 按大小/修改时间/MD5 判断文件的，盲猜按是文件名，备份的话要找别的支持历史版本的玩意（OD/GD）否则没啥意义

我也要了解了解 这个增量备份了 用处真的大

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9346882&amp;ptid=758017" target="_blank"><font color="#999999">kuk 发表于 2020-10-24 18:17</font></a></font><br />
建议多看看官方文档</blockquote></div><br />
很清晰了，多谢！~~

copy只复制缺少的<br />
sync还会检查源头没有的同时删掉目的地的
