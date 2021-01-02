# 硬盘三副本技术


<i class="pstatus"> 本帖最后由 801N 于 2020-11-5 13:54 编辑 </i><br />
<br />
请问硬盘三副本技术属于raid吗？<br />
华为云硬盘三副本：https://support.huaweicloud.com/productdesc-evs/evs_01_0056.html<br />
<br />
<img id="aimg_Hbwxw" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://support.huaweicloud.com/productdesc-evs/zh-cn_image_0205534009.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<img id="aimg_w37AY" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="600" src="https://support.huaweicloud.com/productdesc-evs/zh-cn_image_0205534122.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<br />
阿里云硬盘三副本：https://help.aliyun.com/document_detail/35108.html?spm=5176.10695662.1996646101.searchclickresult.484f2df26yF03e<br />
<img id="aimg_keTy7" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="526" src="https://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/zh-CN/0689205851/p39628.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<img id="aimg_k0bxx" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="146" src="https://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/zh-CN/1689205851/p39629.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<br />
腾讯云普通硬盘应该是没有三副本技术的：https://cloud.tencent.com/document/product/213/43861<br />
<br />
腾讯云便宜一点是不是省材料了，华为云阿里云这么这么贵

炒作概念而已，都是大佬们玩剩下的 <img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" />

怎么大国的厂家总喜欢自己造一些不知所谓的词呢<img id="aimg_NTu1m" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

ceph吧. 很多应用了.

原理类似吧，条带+冗余。但是考虑到集群扩展性应该和raid不完全一样
