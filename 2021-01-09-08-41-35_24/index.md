# 【分享】二字母任意组合列表


啊 怎么突然都秀起代码来了，我是这样写的，方便指定字符<br />
<br /><div class="blockcode"><div id="code_OU9"><ol><li>#!/bin/bash<br /><li>## Useage: https://github.com/Har-Kuun/DomainMegaBot<br /><li>### 生成字典代码<br /><li><br /><li>aword=(a b c d e f g h i j k l m n o p q r s t u v w x y z)<br /><li>bword=(a b c d e f g h i j k l m n o p q r s t u v w x y z)<br /><li>cword=(a b c d e f g h i j k l m n o p q r s t u v w x y z)<br /><li>dword=(a b c d e f g h i j k l m n o p q r s t u v w x y z)<br /><li>eword=(a b c d e f g h i j k l m n o p q r s t u v w x y z)<br /><li><br /><li>for ((i=0; i&lt;${#aword[*]}; i++)); do<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; for ((j=0; j&lt;${#bword[*]}; j++)); do<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; for ((k=0; k&lt;${#cword[*]}; k++)); do<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; for ((l=0; l&lt;${#dword[*]}; l++)); do<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; for ((m=0; m&lt;${#eword[*]}; m++)); do<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; echo ${aword[i]}${bword[j]}${cword[k]}${dword[l]}${eword[m]}<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; done<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; done<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; done<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; done<br /><li>done</ol></div><em onclick="copycode($('code_OU9'));">复制代码</em></div>

我想我可以开一个新帖 分享一下单字母域名的列表&nbsp;&nbsp;

绑定，紫薯布丁
