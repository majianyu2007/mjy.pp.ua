# 问个关于宝塔一键反代缓存的问题


<i class="pstatus"> 本帖最后由 baiyangz1 于 2020-10-27 14:27 编辑 </i><br />
<br />
宝塔设置了一键反代缓存，设置了缓存，网站用的是wordpress，问题来了，wp主题自带的广告功能（标题前、文章后这种简单的插入）分移动端和PC端，现在缓存后，PC端显示的就是移动端的广告，移动端还是移动端，网站是自适应的。求解怎么整。<br />
<br />
补充下，关掉缓存，反代的广告就没问题了。所以怎么在开缓存的情况下没问题呢。

<i class="pstatus"> 本帖最后由 liuyangge 于 2020-10-27 14:54 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359241&amp;ptid=758981" target="_blank"><font color="#999999">baiyangz1 发表于 2020-10-27 14:43</font></a></font><br />
求指导，添加什么代码，纯小白</blockquote></div><br />
<br />
打开配置文件，proxy_cache_key就是缓存key了<br />
可以直接在nginx判断下是否为移动端，然后缓存key增加字段即可<br />
比如将这句话<br /><div class="blockcode"><div id="code_YsD"><ol><li>proxy_cache_key $host$uri$is_args$args;</ol></div><em onclick="copycode($('code_YsD'));">复制代码</em></div><br />
改成这样<br /><div class="blockcode"><div id="code_Sd0"><ol><li>set $ismobile '0';<br /><li>if ($http_user_agent ~* &quot;(mobile|nokia|iphone|ipad|android|samsung|htc|blackberry)&quot;) {<br /><li>&nbsp; &nbsp; set $ismobile '1';<br /><li>}<br /><li>proxy_cache_key $ismobile$host$uri$is_args$args;</ol></div><em onclick="copycode($('code_Sd0'));">复制代码</em></div>

宝塔反代 经常在Safari里打不开网页 

缓存标识改一下，区分下pc端和移动端<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

广告改自适应

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359147&amp;ptid=758981" target="_blank"><font color="#999999">hxuf 发表于 2020-10-27 14:29</font></a></font><br />
广告改自适应</blockquote></div><br />
广告本身就是自适应的，难搞

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359141&amp;ptid=758981" target="_blank"><font color="#999999">liuyangge 发表于 2020-10-27 14:27</font></a></font><br />
缓存标识改一下，区分下pc端和移动端</blockquote></div><br />
求指导，添加什么代码，纯小白

不是自适应模版，静态缓存会好一些，加上伪静态体验也是不错的

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359292&amp;ptid=758981" target="_blank"><font color="#999999">liuyangge 发表于 2020-10-27 14:53</font></a></font><br />
打开配置文件，proxy_cache_key就是缓存key了<br />
可以直接在nginx判断下是否为移动端，然后缓存key增加字段 ...</blockquote></div><br />
有一说一，强的夸张！！！！
