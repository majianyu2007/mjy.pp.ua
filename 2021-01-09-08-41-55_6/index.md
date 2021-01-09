# 小白请问一个CDN的问题


比如网站链接是 <br />
<br />
http://www.abc.com/p/1<br />
http://www.abc.com/p/2<br />
http://www.abc.com/p/3<br />
http://www.abc.com/p/4<br />
<br />
由于是伪静态，所以p后面的数字其实是一个参数，只是把他伪静态话了，也就是是逐步上升的<br />
<br />
<br />
如果在CDN的文件夹那去设置 p/1 这样设置有点不现实。<br />
所有，想问一下，在CDN那要如何设置呢？<br />
<br />
谢谢回答~

文件夹设置/p就可以了，后面的1234都是P文件夹层级下的啊 

设置文件后缀缓存就好了<br />
把css js jpg png等常用的静态文件缓存了，其他的就不会缓存，不会影响网站<br />
<br />
还有，默认不带后缀的话CDN是不会缓存的

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9368180&amp;ptid=759719" target="_blank"><font color="#999999">cheshirex 发表于 2020-10-29 10:56</font></a></font><br />
文件夹设置/p就可以了，后面的1234都是P文件夹层级下的啊</blockquote></div><br />
多谢讲解

可以试试cdn的全站加速或者动态加速

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9368772&amp;ptid=759719" target="_blank"><font color="#999999">流星i 发表于 2020-10-29 12:49</font></a></font><br />
可以试试cdn的全站加速或者动态加速</blockquote></div><br />
我试试看
