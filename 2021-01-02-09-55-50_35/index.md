# 刚刚了解下docker，不知道我这个理解对不对？


docker就是集装箱原理.

<img id="aimg_dC0ab" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://mjj.today/upload/2011/6805d808731727f4.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
非纯表

是这么个意思

docker是個進階版的chroot，大部分人推薦的玩法是php一個容器，mysql一個，nginx再一個容器，全部拆散。不過容器只是技術，你愛怎麼玩怎麼玩。像我都全部放在一起，也不是不行

确实可以这么用<br />
<br />
<br />
​​​​​​​

内存小了，不适合

可以这么理解 <br />
不过你把这些都弄在一个容器里面 不好维护 <br />
还是分开比较好
