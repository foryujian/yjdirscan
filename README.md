## 御剑目录扫描专业版(依赖：Microsoft .NET Framework 4.6.1)
    ★程序使用了壳，可能会造成部分安全软件拦截，如果不放心可以在虚拟机下使用!
    
## 发布：v1.1&nbsp;&nbsp;Date:20201018&nbsp;&nbsp;<a href="../../releases/download/yjdirscan/yjdirscan_v1.1.zip">下载：专业版v1.1</a>
    ★增加存活预判（当目标无法连接3次自动撤销任务）
    ★增加首页爬虫（只抓取首页的目录进行二次扫描）
    ★增加文件存储（可以保存扫描结果到指定文位置）
    ★增加跳过大小（可以设定要忽略的页面大小，min-max）
    ★增加GET模式关键字词组过滤（使用GET模式和关闭自定义404才会生效，可以忽略包含指定关键词的页面）
    ★默认参数和值相对更加合理的初始化（不合理的设置会导致目标产生CC或者漏报）
    ★优化扫描速度（比1.0提升速度大概5-10倍，通过maxspeed参数控制速度最大值）
    ★优化内存占用（1000/s内存占用10-30M左右）

## 发布：v1.0&nbsp;&nbsp;Date:20201005&nbsp;&nbsp;<a href="../../releases/download/yjdirscan/yjdirscan.zip">下载：专业版v1.0</a>
    ★支持修改UserAgent
    ★支持开启和关闭自定义404识别
    ★支持控速
    ★支持fuzz和字典扫描模式
    ★支持字典变量
## 示例：
命令行程序：yjdirscan.exe -h

Program:
     yjdirscan(御剑目录扫描专业版v1.1 Date:20201018)

Usage:
     -url https://www.demo.com
     -url https://www.demo.com -method GET -diy404 off -skipword not found   explain:use skip word mode(解释:启用关键词跳过模式)
     -fuzz https://www.demo.com/*/ -range 1,3
     -fuzz https://www.demo.com/admin/*.zip -range 3,3

Options:
     -check     Check Url State Failed Three Exit Scan,Default on/off
     -spider    Home Page Spider,Default on/off
     -diy404    Auto Filter Diy404(False200),Default on/off
     -method    HEAD or GET,Default HEAD
     -thread    1-100,Default 16
     -timeout   1000-60000,Default 6000
     -maxspeed  1-3000,Default 200
     -codes     httpcode,Default 200,301,302,304,403
     -files     all or xxx.txt,Default bak.txt,dir.txt
     -key       fuzz mode,Default abcdefghijklmnopqrstuvwxyz
     -range     fuzz mode,Default 1,3
     -save      Save to xxx.txt File,Default Not Save
     -skipsize  Skip Page size-size,Default Not use
     -skipword  method is GET and diy404 is off use,Default not found

Dicvar(bak.txt):
     www.demo.com  Split(3)  www=%a% demo=%b% com=%c%
         demo.com  Split(2)          demo=%b% com=%c%
     
## 截图：
<img src="https://github.com/foryujian/yjdirscan/blob/main/img/404.png" width="600px" height="400px"/><br>
<img src="https://github.com/foryujian/yjdirscan/blob/main/img/dicscan.png" width="600px"  height="400px"/><br>
<img src="https://github.com/foryujian/yjdirscan/blob/main/img/fuzzscan.png" width="600px"  height="400px"/><br>
