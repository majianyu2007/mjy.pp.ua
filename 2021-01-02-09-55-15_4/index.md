# BuyVM可以把系统装到存储块里


<i class="pstatus"> 本帖最后由 zutianrun 于 2020-10-22 12:15 编辑 </i><br />
<br />
<img id="aimg_U8uAh" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/22/Hgm3eLxSMU4PBYG.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
<font size="5">虽然没什么用</font> <img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /> <br />
<br />
<font size="3">1.挂iso装系统<br />
2.安装winpe到系统盘，根目录找到winpe.wim，用WimTool把virtio驱动打进去<br />
3.重启进pe (VNC)，打上硬盘驱动，分区助手克隆系统盘到存储块，重启<br />
4.bootice-&gt;选中原系统盘(不是存储块)-&gt;主引导记录-&gt;wee-&gt;<br />
<br />
timeout 0<br />
default 0<br />
title 1. Windows<br />
find --set-root --active command +1<br />
find --set-root (hd0,0)/bootmgr /bootmgr<br />
find --set-root (hd0,0)/ntldr /ntldr<br />
<br />
<br />
</font>

装在存储盘里面。内存是怎么算的。 在线率高么。拿去挂采集器

大佬厉害，会玩！<br />
<br />
这样的话，更多人要买了吧<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

装个双系统

这个很有用啊，可以把原来的ssd做bcache来提高存储块的读写性能

处理器居然是3900X，香啊
