# 安装锐速有这么玄学么？


已经安装锐速内核，但是无法锐速加速模块<br />
<img id="aimg_bvhqH" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://tu.sunpma.com/imgs/2020/10/b7cc7e409d7fbbe0.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
提示Error! I can not generate the Lic for you<br />
<img id="aimg_huVQ6" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://tu.sunpma.com/imgs/2020/10/d18eec463fc62792.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
<br />
同样DD debian9 ，同样的脚本，不同家的小鸡有的能装上锐速，有的死活都装不上。求大佬指导<br />
<br />
尝试脚本：<br /><div class="blockcode"><div id="code_k8o"><ol><li>wget -N --no-check-certificate &quot;https://github.000060000.xyz/tcpx.sh&quot; &amp;&amp; chmod +x tcpx.sh &amp;&amp; ./tcpx.sh</ol></div><em onclick="copycode($('code_k8o'));">复制代码</em></div><br />
<div class="blockcode"><div id="code_hUd"><ol><li>bash &lt;(wget --no-check-certificate -qO- https://github.com/Meilinhost/LotServer_Vicer/raw/master/Install.sh) install</ol></div><em onclick="copycode($('code_hUd'));">复制代码</em></div><br />
<div class="blockcode"><div id="code_DFf"><ol><li>bash &lt;(wget --no-check-certificate -qO- https://github.com/iiiiiii1/LotServer/raw/master/Install.sh) install</ol></div><em onclick="copycode($('code_DFf'));">复制代码</em></div><br />
<br />


装锐速毛病很多。。。。

锐速占用特别大，先free -m 看看内存够不够

debian用 bbrp，centos用锐速<br />
辣鸡vps用fs双边抢救<br />
<br />
锐速一键其实都是萌卡的那个吧

锐速确实有的鸡装不上 没办法啊

不顶 帮懂<img src="static/image/smiley/yct/013.gif" smilieid="43" border="0" alt="" />

无脑BBR

我都装原版BBR

很多鸡换不了内核

<i class="pstatus"> 本帖最后由 kra 于 2020-10-30 17:31 编辑 </i><br />
<br />
在不同商家的使用 ，试验。<br />
wget -N --no-check-certificate &quot;https://github.000060000.xyz/tcpx.sh&quot; &amp;&amp; chmod +x tcpx.sh &amp;&amp; ./tcpx.sh<br />
的方式都可以安装成功。<br />
<br />
安装锐速不行的是哪家主机？<br />

