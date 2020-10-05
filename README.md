# yjdirscan 御剑目录扫描专业版v1.0 Date:20201005
## 依赖.net framework 4.6.1或者更高的版本！<br>

#### ★支持UserAgent自定义,通过修改files\useragent.ini生效<br>
#### ★支持开启和关闭自定义404识别<br>
#### ★支持限速<br>
#### ★支持fuzz扫描模式<br>
#### ★支持字典变量<br>

#### 示例<br>
Program:<br>
     yjdirscan(御剑目录扫描专业版v1.0 Date:20201005)<br>
<br>
Usage:<br>
     -url https://www.demo.com<br>
     -fuzz https://www.demo.com/admin/*.zip -range 3,3<br>
<br>
Options:<br>
     -thread      1-100,Default 4<br>
     -timeout     1000-60000,Default 6000<br>
     -maxspeed    1-1000,Default 200<br>
     -method      HEAD or GET,Default HEAD<br>
     -diy404      on or off,Default on<br>
     -codes       httpcode,Default 200,301,302,304,403<br>
     -files       all or File,Default bak.txt,dir.txt<br>
     -key         fuzz mode,Default abcdefghijklmnopqrstuvwxyz<br>
     -range       fuzz mode,Default 1,3<br>
<br>
Dicvar(bak.txt):<br>
     www.demo.com Split(3)  www=%a% demo=%b% com=%c%<br>
     demo.com     Split(2)          demo=%b% com=%c%<br>

![](https://github.com/foryujian/yjdirscan/blob/main/404.png)<br>

![](https://github.com/foryujian/yjdirscan/blob/main/c1.png)<br>

![](https://github.com/foryujian/yjdirscan/blob/main/dicscan.png)<br>

![](https://github.com/foryujian/yjdirscan/blob/main/fuzzscan.png)<br>
