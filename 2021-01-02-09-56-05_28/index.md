# 关于甲骨文


关于甲骨文各种坑官方解释：<br />
<br />
计算<br />
所有租约都有两个Always Free Compute虚拟机（VM）实例。<br />
<br />
您必须在本地区域中创建Always Free Compute实例。<br />
<br />
Always Free Compute实例的详细信息<br />
形状：&nbsp;&nbsp;VM.Standard.E2.1.Micro<br />
处理器： OCPU的1/8，可以使用其他CPU资源<br />
记忆体： 1 GB<br />
联网： 包括一个VNIC&nbsp;&nbsp;具有一个公共IP地址和高达480 Mbps的网络带宽<br />
操作系统： 您选择下列始终免费的合格操作系统之一：<br />
<br />
Oracle Linux（包括Oracle自治Linux）<br />
规范的Ubuntu Linux<br />
CentOS Linux<br />
<br />
标记为“始终免费合格”的Linux操作系统与Always Free Compute实例兼容，并且不会产生任何许可费用。这些操作系统还与付费资源兼容，并且可供付费帐户的用户使用。要使用不总是免费的合格操作系统配置Compute实例，您必须具有付费帐户或具有可用信用的免费试用帐户。<br />
<br />
<br />
块体积<br />
所有租约将获得总共100 GB的“始终可用的块卷”存储和五个卷备份。这些数量适用于引导卷和块卷的总和。设置Compute实例时，该实例会自动收到50 GB的启动卷进行存储。您还可以创建和附加块卷以扩展Compute实例的存储容量。有关更多信息，请参见创建卷和附加卷。<br />
<br />
Always Free Block Volume资源的详细信息<br />
总共100 GB的引导卷和块卷的总和 。Always Free 块卷存储。<br />
<br />
五份总卷备份（引导卷和块卷的总和）。<br />
创建Compute实例时，该实例的默认启动卷大小为50 GB，这将计入您分配的100 GB。您可以自定义实例的启动卷大小，最大为100 GB。但是，这将用尽您的全部存储空间分配给Always Free Block Volume资源。此外，由于Compute实例允许的最小启动卷大小为50 GB，因此启动两个实例将使用您的所有Always Free Block Volume资源。或者，您可以启动默认启动卷大小为50 GB的一个实例，然后创建并附加一个50 GB的块卷以扩展该实例的存储容量。有关更多信息，请参见创建卷和附加卷。尽管可以混合使用付费资源和“永远免费”资源，但是Oracle不建议这样做。如果您已经用完了“始终释放的 块卷”资源的分配，则可以通过终止“始终释放”的实例并删除启动卷，或者终止“始终释放的”块卷来释放块存储资源。<br />
<br />
任何时候最多可以有五个Always Free卷备份。这适用于启动卷备份和块卷备份。例如，你可以有你的三个启动卷备份永远免费实例，并为您的两块卷备份永远免费块卷。在此示例中，如果尝试创建新备份，则操作将失败并显示错误，直到您删除现有的Always Free卷备份。有关卷备份的详细信息，请参阅阻止卷备份的概述和引导概述卷备份。<br />
<br />
<br />
30天试用结束以后一定要检查使用储存是不是超过100G，备份也算在内的，必须要显示始终免费才算数·····································

别开超过两台免费机不就行了

太长不看，反正已经存活7个月了。<img id="aimg_ltMS3" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

我已经用了一年多了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

已经超过一年了

已经超过15年了

能不能说点能看懂的话
