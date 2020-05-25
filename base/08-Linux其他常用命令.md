## Linux其他常用命令

### awk
#### awk作用
awk是处理文本文件的工具，名字取自三个人的名字首字母
 * awk 【选项参数】 'script' var=value file(s)
 * awk 【选项参数】-f scriptfile var=value file(s)
 
 * awk '{print $1, $3}' log.txt 每行按空格分割，输出文本中第1，3项
 * awk -F , '{print $1, $3}' log.txt 按照'，'进行分割，输出1，3项
 * awk -va=1 '{print $1, $3 + a}' log.txt 
 设置变量a=1，让第三项加a
 
### netstat
netstat用于显示网络状态，包括端口和进程等信息
 * netstat -ntlp  查看当前所有tcp端口
 * netstat -an|grep 3306    查看所有3306端口使用情况
 * netstat -ano     显示tcp／ip网络连接情况