# 请教一个PT下载的问题


应该就是权限问题，我以前遇到过<br />
你用的是docker还是直接安装的

我想知道你们玩pt到底是为了个什么&nbsp; &nbsp;

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349602&amp;ptid=758239" target="_blank"><font color="#999999">鼎剑阁 发表于 2020-10-25 13:23</font></a></font><br />
应该就是权限问题，我以前遇到过<br />
你用的是docker还是直接安装的</blockquote></div><br />
docker

推荐用 qb 个人感觉比 tr 方便

直接用PT Master不香吗

看不清图，两种可能的纠错方法：<br />
1. 点那个暂停的种子，再点下方一个偏浅蓝色的长条弹出上拉菜单，再看下“常规”，“服务器”， “文件”等选项卡里是否显示详细的异常消息<br />
2. check种子的已完成大小，是否和你的缓存大小一致，如果是的话大概率是transmission无法写入到你的下载目录，手动cd到下载目录下sudo -u transmission touch testfile 试一下

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349629&amp;ptid=758239" target="_blank"><font color="#999999">shuohaobulude 发表于 2020-10-25 13:32</font></a></font><br />
docker</blockquote></div><br />
那就是了，我之前也是docker出现了这个问题。<br />
比如你的启动参数是<br />
-v ~/transmission/config:/config \<br />
-v ~/transmission/downloads:/downloads \<br />
-v ~/transmission/watch:/watch \<br />
把~/transmission/downloads这个目录及子目录赋予777权限

是不是硬盘没开权限
