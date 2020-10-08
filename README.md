# 御剑目录扫描专业版v1.0(Date:20201005)<br>
#### ★支持修改UserAgent<br>
#### ★支持开启和关闭自定义404识别<br>
#### ★支持限速<br>
#### ★支持fuzz和字典扫描模式<br>
#### ★支持字典变量<br>

<font color='red'> text </font>

#### 示例<br>
* Program:
     > yjdirscan(御剑目录扫描专业版v1.0 Date:20201005)
* Usage:
     > -url&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;https://www.demo.com<br>
     > -fuzz&nbsp;&nbsp;&nbsp;https://www.demo.com/admin/*.zip -range 3,3
* Options:
     > -thread&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1-100,Default 4<br>
     > -timeout&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1000-60000,Default 6000<br>
     > -maxspeed&nbsp;1-1000,Default 200<br>
     > -method&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HEAD or GET,Default HEAD<br>
     > -diy404&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;on or off,Default on<br>
     > -codes&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;httpcode,Default 200,301,302,304,403<br>
     > -files&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;all or File,Default bak.txt,dir.txt<br>
     > -key&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;fuzz mode,Default abcdefghijklmnopqrstuvwxyz<br>
     > -range&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;fuzz mode,Default 1,3
* Dicvar(bak.txt):
     > www.demo.com Split(3)  www=%a% demo=%b% com=%c%<br>
     > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;demo.com Split(2)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;demo=%b% com=%c%

<img src="https://github.com/foryujian/yjdirscan/blob/main/img/404.png" width="800px" height="400px"/><br>
<img src="https://github.com/foryujian/yjdirscan/blob/main/img/c1.png" width="800px"  height="400px"/><br>
<img src="https://github.com/foryujian/yjdirscan/blob/main/img/dicscan.png" width="800px"  height="400px"/><br>
<img src="https://github.com/foryujian/yjdirscan/blob/main/img/fuzzscan.png" width="800px"  height="400px"/><br>
