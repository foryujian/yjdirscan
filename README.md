# yjdirscan 御剑目录扫描专业版v1.0 Date:20201005
C:\Users\Administrator>yjdirscan.exe
Usage:
     -url https://www.demo.com
     -fuzz https://www.demo.com/admin/*.zip -range 3,3

Options:
     -thread      1-100,Default 4
     -timeout     1000-60000,Default 6000
     -maxspeed    1-1000,Default 200
     -method      HEAD or GET,Default HEAD
     -diy404      on or off,Default on
     -codes       httpcode,Default 200,301,302,304,403
     -files       all or File,Default bak.txt,dir.txt
     -key         fuzz mode,Default abcdefghijklmnopqrstuvwxyz
     -range       fuzz mode,Default 1,3

Dicvar(bak.txt):
     www.demo.com Split(3)  www=%a% demo=%b% com=%c%
     demo.com     Split(2)          demo=%b% com=%c%
     
     
★支持UserAgent自定义,通过修改files\useragent.ini生效
★支持开启和关闭自定义404识别
★支持限速
★支持fuzz扫描模式
★支持字典变量

依赖：
.net framework 4.6.1或者更高的版本！
