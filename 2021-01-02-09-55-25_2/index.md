# 谷歌浏览器怎么关闭网页的弹窗提示？


<i class="pstatus"> 本帖最后由 爱吃醋的醋醋 于 2020-10-23 11:06 编辑 </i><br />
<br />
<img id="aimg_gnN4n" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://p.pstatp.com/origin/137a50001e316aeb8cfab" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
谷歌浏览器怎么关闭网页的弹窗提示？<br />
<br />
很烦，只能点确定<br />
<br />
怎么关闭这种提示框

多弹几个，chrome就会多一个复选框，允许你禁止再显示类似的窗口

可以试试在控制台重写alert<br /><div class="blockcode"><div id="code_fuh"><ol><li>window.alert = msg=&gt;undefined;</ol></div><em onclick="copycode($('code_fuh'));">复制代码</em></div>
