## Linux压缩打包
### zip 用来压缩文件
 * zip -q -r html.zip /home/html
 -q 不显示指令执行过程，
 -r 递归处理，将指定目录下的文件和子目录一并处理
### unzip 用来解压文件
 * unzip test.zip 
 
### gzip 用来压缩文件
 * gzip *    将当前目录下的每个文件都压缩成.gz文件
 * gzip test    将test文件压缩成test.gz并删除原文件
 * gzip -rv ／tmp    递归压缩文件及目录，并显示指令执行过程
 * gzip -dr ／tmp    递归解压／tmp目录下的.gz结尾的文件
 
### gunzip 用来解压文件
 * gzip -d test.gz 
 * gunzip test.gz   这两个命令效果一样
 
### tar 可以为Linux的文件和目录创建档案，
tar用于打包，并不压缩
利用 tar 命令可以将文件或目录打包成一个文件，便于备份或传输
 * tar -cvf log.tar log22.log   仅打包，不压缩
 * tar -xf log.tar 解压
 * tar -zcvf log.tar.gz log22.log 打包后，以gzip压缩
 * tar -zxf log.tar.gz 解压   后面两个命令常用