# 采集好了bing图片，不过在自动发布到网站有问题


<br />
<br />
<a href="https://www.daydaypic.com" target="_blank">https://www.daydaypic.com</a><br />
<br />
<br />
从之前MJJ说的网站采集的，从2016年3月到今天的，一千多天的图片<br />
<br />
<br />
现在只要每天从bing采集发布就行了<br />
<br />
<br />
不过写的脚本手动执行没问题，但写到crontab就不行了，路径都是绝对路径，应该没问题才对<br />
<br />
<br />
但是hexo生成部署的时候报错了(手动执行脚本不报)，百度没搜到这个的类似情况，大概是hexo的依赖问题？<br />
<br />
<br /><div class="blockcode"><div id="code_z41"><ol><li>/usr/local/lib/node_modules/hexo-cli/node_modules/chalk/source/index.js:106<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;...styles,<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;^^^<br /><li><br /><li>SyntaxError: Unexpected token ...<br /><li>&nbsp; &nbsp; at createScript (vm.js:56:10)<br /><li>&nbsp; &nbsp; at Object.runInThisContext (vm.js:97:10)<br /><li>&nbsp; &nbsp; at Module._compile (module.js:549:28)<br /><li>&nbsp; &nbsp; at Object.Module._extensions..js (module.js:586:10)<br /><li>&nbsp; &nbsp; at Module.load (module.js:494:32)<br /><li>&nbsp; &nbsp; at tryModuleLoad (module.js:453:12)<br /><li>&nbsp; &nbsp; at Function.Module._load (module.js:445:3)<br /><li>&nbsp; &nbsp; at Module.require (module.js:504:17)<br /><li>&nbsp; &nbsp; at require (internal/module.js:20:19)<br /><li>&nbsp; &nbsp; at Object.&lt;anonymous&gt; (/usr/local/lib/node_modules/hexo-cli/lib/hexo.js:3:15)<br /><li></ol></div><em onclick="copycode($('code_z41'));">复制代码</em></div><br />
<br />
<br />
<img id="aimg_SZ302" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://developer-forum-online.cdn.bcebos.com/b13735be-4492-48aa-901c-e7c6a6208db7.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />


l路径问题，<br />
“crontab执行shell时，是不会进入到shell脚本所在的路径下执行的，如果shell里含有相对路径的话，会找不到路径的，因此shell脚本中都要使用绝对路径。”<br />
<br />
使用 cd /home/ &amp;&amp; ./hexo

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9379934&amp;ptid=760533" target="_blank"><font color="#999999">robot 发表于 2020-10-31 11:52</font></a></font><br />
l路径问题，<br />
“crontab执行shell时，是不会进入到shell脚本所在的路径下执行的，如果shell里含有相对路径的 ...</blockquote></div><br />
应该不是路径问题。一开始我就路径问题进行了排查，将shell脚本内有需要的的路径都改为绝对路径了，有需要cd的目录都cd了(hexo目录和vercel目录)。后面甚至还在脚本开头加载了/etc/profile
