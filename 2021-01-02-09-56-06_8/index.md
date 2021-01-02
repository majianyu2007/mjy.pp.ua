# 问个nginx的问题


在www.a.com上的nginx， 怎么写才能匹配到， 把请求转发到www.b.com的机器上呢？<br /><div class="blockcode"><div id="code_qIr"><ol><li><br /><li>http://www.a.com/js/app.js<br /><li> ||<br /><li> \/<br /><li>http://www.b.com/www.a.com/js/app.js<br /><li></ol></div><em onclick="copycode($('code_qIr'));">复制代码</em></div>

这有难度？<br /><div class="blockcode"><div id="code_Qdi"><ol><li>server {<br /><li>&nbsp; &nbsp; listen 80;<br /><li>&nbsp; &nbsp; listen [::]:80;<br /><li><br /><li>&nbsp; &nbsp; server_name www.a.com;<br /><li><br /><li>&nbsp; &nbsp; return 301 http://www.b.com/www.a.com$request_uri;<br /><li>}</ol></div><em onclick="copycode($('code_Qdi'));">复制代码</em></div><img id="aimg_FeNq3" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

rewrite
