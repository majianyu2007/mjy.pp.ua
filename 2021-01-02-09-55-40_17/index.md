# 买了一套JAVA的源码，编译的时候报错，有没有大佬帮忙看下


<i class="pstatus"> 本帖最后由 tian1781 于 2020-10-25 12:01 编辑 </i><br />
<br />
感谢大佬们，已经解决<br />


看起来像是问道的手游服务端？还是windows端

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349230&amp;ptid=758229" target="_blank"><font color="#999999">ssjoy 发表于 2020-10-25 11:44</font></a></font><br />
看起来像是问道的手游服务端？还是windows端</blockquote></div><br />
java 都可以装 跨平台的

用oracle jdk&nbsp;&nbsp;然后注意版本

jdk版本不一致

执行预编译任务...加载Ant配置...运行Ant任务...运行'之前'任务检查源复制资源... [asktaoGameServer]解析java ... [asktaoGameServer] java：编译模块时发生错误'asktaoGameServer'正在检查依赖项... [asktaoGameServer]依赖关系分析发现0个受影响的文件javac 11用于编译Java源代码已完成，正在保存缓存...编译失败：错误：1;警告：1执行编译后任务...加载Ant配置...运行Ant任务...同步输出目录... 2020/10/25 11:37-构建完成，在20 s内有1个错误和1个警告ms D：\ wd \ asktaoGameServer \ src \ main \ java \ org \ linlinjava \ litemall \ gameserver \ process \ CMD_SELECT_MENU_ITEM.java：42 java：字段'log'已经存在。D：\ wd \ asktaoGameServer \ src \ main \ java \ org \ linlinjava \ litemall \ wx \ util \ Aes.java：5：16 java：程序包sun.misc不存在

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349245&amp;ptid=758229" target="_blank"><font color="#999999">xuh 发表于 2020-10-25 11:47</font></a></font><br />
jdk版本不一致</blockquote></div><br />
大佬 知道怎么查看他的jdk的版本么 

sun.misc用jdk1.7或者1.8，最好1.8吧<br />
sun.misc在1.8以后的版本弃用了，属于内部接口

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349285&amp;ptid=758229" target="_blank"><font color="#999999">ABCHINA 发表于 2020-10-25 11:55</font></a></font><br />
sun.misc用jdk1.7或者1.8，最好1.8吧<br />
sun.misc在1.8以后的版本弃用了，属于内部接口 ...</blockquote></div><br />
好的 已经解决了 谢谢
