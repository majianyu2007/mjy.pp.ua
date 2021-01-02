# 救救孩子怎么写python自动签到脚本


<br />
求python大佬救救孩子<img src="static/image/smiley/yct/002.gif" smilieid="30" border="0" alt="" /> ，每天打卡签到太难受了<br />
想实现python自动签到脚本遇到一些问题，request的post不知道怎么写data字典来选中一个滚动选择的地区如选择成都市武侯区（网页源码为第一部分），第二个怎么实现点击checkbox使得button可以不再是disable（网页源码见第二部分），从而实现自动提交。<img src="static/image/smiley/yct/019.gif" smilieid="49" border="0" alt="" /> <br />
<br />
第一部分<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&lt;select name=&quot<img src="static/image/smiley/default/titter.gif" smilieid="9" border="0" alt="" />rovince&quot; onchange=&quot<img src="static/image/smiley/default/titter.gif" smilieid="9" border="0" alt="" />rovinceChange(this);&quot; class=&quot;select-style required validate&quot;&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&lt;option value=&quot;&quot;&gt;&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;110000&quot;&gt;北京市&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;120000&quot;&gt;天津市&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;130000&quot;&gt;河北省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;140000&quot;&gt;山西省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;150000&quot;&gt;内蒙古自治区&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;210000&quot;&gt;辽宁省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;220000&quot;&gt;吉林省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;230000&quot;&gt;黑龙江省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;310000&quot;&gt;上海市&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;320000&quot;&gt;江苏省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;330000&quot;&gt;浙江省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;340000&quot;&gt;安徽省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;350000&quot;&gt;福建省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;360000&quot;&gt;江西省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;370000&quot;&gt;山东省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;410000&quot;&gt;河南省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;420000&quot;&gt;湖北省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;430000&quot;&gt;湖南省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;440000&quot;&gt;广东省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;450000&quot;&gt;广西壮族自治区&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;460000&quot;&gt;海南省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;500000&quot;&gt;重庆市&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;510000&quot; selected=&quot;selected&quot;&gt;四川省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;520000&quot;&gt;贵州省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;530000&quot;&gt;云南省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;540000&quot;&gt;西藏自治区&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;610000&quot;&gt;陕西省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;620000&quot;&gt;甘肃省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;630000&quot;&gt;青海省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;640000&quot;&gt;宁夏回族自治区&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;650000&quot;&gt;新疆维吾尔自治区&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;710000&quot;&gt;台湾省&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;810000&quot;&gt;香港特别行政区&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;820000&quot;&gt;澳门特别行政区&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; &lt;option value=&quot;990000&quot;&gt;国外&lt;/option&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&lt;/select&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&lt;select name=&quot;City&quot; onchange=&quot;CityChange(this);&quot; class=&quot;select-style required validate&quot;&gt;&lt;option value=&quot;&quot;&gt;&lt;/option&gt;&lt;option value=&quot;510100&quot;&gt;成都市&lt;/option&gt;&lt;option value=&quot;510300&quot;&gt;自贡市&lt;/option&gt;&lt;option value=&quot;510400&quot;&gt;攀枝花市&lt;/option&gt;&lt;option value=&quot;510500&quot;&gt;泸州市&lt;/option&gt;&lt;option value=&quot;510600&quot;&gt;德阳市&lt;/option&gt;&lt;option value=&quot;510700&quot;&gt;绵阳市&lt;/option&gt;&lt;option value=&quot;510800&quot;&gt;广元市&lt;/option&gt;&lt;option value=&quot;510900&quot;&gt;遂宁市&lt;/option&gt;&lt;option value=&quot;511000&quot;&gt;内江市&lt;/option&gt;&lt;option value=&quot;511100&quot;&gt;乐山市&lt;/option&gt;&lt;option value=&quot;511300&quot;&gt;南充市&lt;/option&gt;&lt;option value=&quot;511400&quot;&gt;眉山市&lt;/option&gt;&lt;option value=&quot;511500&quot;&gt;宜宾市&lt;/option&gt;&lt;option value=&quot;511600&quot;&gt;广安市&lt;/option&gt;&lt;option value=&quot;511700&quot;&gt;达州市&lt;/option&gt;&lt;option value=&quot;511800&quot;&gt;雅安市&lt;/option&gt;&lt;option value=&quot;511900&quot;&gt;巴中市&lt;/option&gt;&lt;option value=&quot;512000&quot;&gt;资阳市&lt;/option&gt;&lt;option value=&quot;513200&quot;&gt;阿坝藏族羌族自治州&lt;/option&gt;&lt;option value=&quot;513300&quot;&gt;甘孜藏族自治州&lt;/option&gt;&lt;option value=&quot;513400&quot;&gt;凉山彝族自治州&lt;/option&gt;&lt;/select&gt;<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&lt;select name=&quot;County&quot; class=&quot;select-style required validate&quot;&gt;&lt;option value=&quot;&quot;&gt;&lt;/option&gt;&lt;option value=&quot;510104&quot;&gt;锦江区&lt;/option&gt;&lt;option value=&quot;510105&quot;&gt;青羊区&lt;/option&gt;&lt;option value=&quot;510106&quot;&gt;金牛区&lt;/option&gt;&lt;option value=&quot;510107&quot;&gt;武侯区&lt;/option&gt;&lt;option value=&quot;510108&quot;&gt;成华区&lt;/option&gt;&lt;option value=&quot;510112&quot;&gt;龙泉驿区&lt;/option&gt;&lt;option value=&quot;510113&quot;&gt;青白江区&lt;/option&gt;&lt;option value=&quot;510114&quot;&gt;新都区&lt;/option&gt;&lt;option value=&quot;510115&quot;&gt;温江区&lt;/option&gt;&lt;option value=&quot;510116&quot;&gt;双流区&lt;/option&gt;&lt;option value=&quot;510117&quot;&gt;郫都区&lt;/option&gt;&lt;option value=&quot;510121&quot;&gt;金堂县&lt;/option&gt;&lt;option value=&quot;510129&quot;&gt;大邑县&lt;/option&gt;&lt;option value=&quot;510131&quot;&gt;蒲江县&lt;/option&gt;&lt;option value=&quot;510132&quot;&gt;新津县&lt;/option&gt;&lt;option value=&quot;510181&quot;&gt;都江堰市&lt;/option&gt;&lt;option value=&quot;510182&quot;&gt;彭州市&lt;/option&gt;&lt;option value=&quot;510183&quot;&gt;邛崃市&lt;/option&gt;&lt;option value=&quot;510184&quot;&gt;崇州市&lt;/option&gt;&lt;option value=&quot;510185&quot;&gt;简阳市&lt;/option&gt;&lt;/select&gt;<br />
<br />
<br />
<br />
<br />
第二部分<br />

<ignore_js_op>

<img id="aimg_140733" aid="140733" src="static/image/common/none.gif" zoomfile="forum.php?mod=attachment&aid=MTQwNzMzfDllZmU0MTFmfDE2MDk1MjQ2MTZ8NDczNDR8NzU4MjI1&noupdate=yes&nothumb=yes" file="forum.php?mod=attachment&aid=MTQwNzMzfDllZmU0MTFmfDE2MDk1MjQ2MTZ8NDczNDR8NzU4MjI1&noupdate=yes" class="zoom" onclick="zoom(this, this.src, 0, 0, 0)" width="347" id="aimg_140733" inpost="1" onmouseover="showMenu({'ctrlid':this.id,'pos':'12'})" />

<div class="tip tip_4 aimg_tip" id="aimg_140733_menu" style="position: absolute; display: none" disautofocus="true">
<div class="xs0">
<p><strong>chpng.png</strong> <em class="xg1">(48.85 KB, 下载次数: 0)</em></p>
<p>
<a href="forum.php?mod=attachment&amp;aid=MTQwNzMzfDllZmU0MTFmfDE2MDk1MjQ2MTZ8NDczNDR8NzU4MjI1&amp;nothumb=yes" target="_blank">下载附件</a>

</p>

<p class="xg1 y">2020-10-25 11:34 上传</p>

</div>
<div class="tip_horn"></div>
</div>

</ignore_js_op>


<img src="static/image/smiley/default/titter.gif" smilieid="9" border="0" alt="" />表情为怎么P

不会，绑定，楼下来<img id="aimg_zowCc" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

这是签到什么东西？<br />
<br />
还全国各省啊！<br />
<br />
<img src="static/image/smiley/default/shocked.gif" smilieid="6" border="0" alt="" /><img src="static/image/smiley/default/shocked.gif" smilieid="6" border="0" alt="" /><img src="static/image/smiley/default/shocked.gif" smilieid="6" border="0" alt="" />

你f12看，network里面的post地址

抓包啊 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349197&amp;ptid=758225" target="_blank"><font color="#999999">Uler 发表于 2020-10-25 11:38</font></a></font><br />
你f12看，network里面的post地址</blockquote></div><br />
全是get

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349204&amp;ptid=758225" target="_blank"><font color="#999999">kuzz_maker 发表于 2020-10-25 11:40</font></a></font><br />
抓包啊</blockquote></div><br />
抓了，但是用包里没有点击的value

不会，绑定
