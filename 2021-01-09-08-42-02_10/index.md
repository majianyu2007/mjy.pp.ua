# 有没有达人知道有没有什么扫描工具只要知道他端口通不通


不用特别功能，只要能扫出他哪些端口是通的就行。 x-scan 太慢了。扫一台6W多端口要很久。

64位下载地址：https://www.lanzoux.com/iVfLTghv3cj<br />
32位下载地址：https://www.lanzoux.com/if21zghv3mj

你需要这个。 https://github.com/robertdavidgraham/masscan

nmap不就行，，，

太快容易漏<img id="aimg_Y87X7" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 sleeli 于 2020-10-30 09:10 编辑 </i><br />
<br />
nc 命令呀<br />
端口扫描 可以执行：<br />
nc -v -w 1 192.168.228.222 -z 1-1000

Port scan

nmap ，最快的<img id="aimg_INrHt" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
