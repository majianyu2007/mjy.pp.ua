# 有没有那种一键压缩视频的软件？


就是那种不要选任何参数的，直接选压缩后质量的，和压缩图片一样，只选择高中低质量，然后一键压缩变小

<i class="pstatus"> 本帖最后由 sRGB 于 2020-10-27 10:41 编辑 </i><br />
<br />
使用 ffmpeg 压缩，指定预置参数<br />
叫大佬写个脚本就行<br />
<br />
<br />
使用 FFMPEG 转 H265 减小文件大小<br />
ffmpeg -i input.mp4 -c:v libx265 -crf 30 -map 0:v -map 0:a:0 output.mp4 <br />
<br />
crf越高,压缩率越高,值是30-100<br />
<br />
可以在这个基础上改改

ShanaEncoder5.1.0.2<br />
还有个B站用的小什么

QQ影音&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;ZSBD

小丸工具箱&nbsp;&nbsp;最新版本16年更新的，之前一直用的这个

有在线版的，之前用过一个shipinyasuo点com，不过会根据压缩大小来收费下载，同类产品挺多的

格式工厂有有各种预设！
