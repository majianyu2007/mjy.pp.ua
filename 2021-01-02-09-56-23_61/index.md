# 问各位Office订阅管理员大佬们一个API权限问题


自己手里有个E3 MSDN订阅，默认Onemanager申请tokenID一直失败，返回null 0。自己手动在Azure活动目录上自己申请应用ID在手动填入客户端ID和密钥就一次成功。<br />
这里延伸出一个问题，我在 Azure Active Directory网页上——企业应用程序——用户设置中如图这样设置，其中“用户可以请求管理员同意他们无法同意的应用”我选了否，怀疑是不是这里选择权限出了问题导致Onemanager集成失败。<br />
<img id="aimg_rhqGI" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://hk2g.video233.tk/Azure.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
各位大佬能截下你们这里权限的图吗,能够正常使用Onemanager中自动申请API Token的设置图，谢谢！<br />


对的，应该要选“是”！<br />
<br />
我的理解是这样<br />
<br />
如果错误，请大佬们见谅！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

onemanager不是自带Api么
