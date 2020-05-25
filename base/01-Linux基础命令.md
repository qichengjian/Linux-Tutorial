# Linux基础命令

## 常用命令
### ls 
 * ls 查看当前目录
 * ls -l 查看当前目录并列出文件属性
### cd
 * cd 切换目录
 * cd ～ 当前用户的家目录
 * cd . 当前目录
 * cd .. 上一层目录
 * cd - 回到上一次所在目录
### pwd
 * pwd 显示当前所在位置绝对路径
### mkdir
 * mkdir 【directory】创建目录
 * mkdir -p 【directory/directory】创建多级目录
### touch
 * touch 【filename】 创建文件
### rm
 * rm 【filename】 删除文件
 * rm -rf 强制递归删除
 * rm -r 【directory】 删除目录及目录下的文件
### cp
 * cp 原文件 目的地 复制原文件到目的地
### mv
 * mv 原文件 目的地 移动源文件到目的地

##查看文件内容
### cat
 * cat -n 【filename】  查看小文件并显示行号
 * cat -n 20 【filename】 查看小文件前20行并显示行号
### tac
 * tac -n 【filename】以倒序查看文件 
### head
 * head 【filename】 从头开始查看文件
 * head -n 20 【filename】 从头开始查看大文件前20行
### tail
 * tail 【filename】 从尾开始查看文件
 * tail -n 20 【filename】 从尾开始查看大文件20行
### more
 * more 【filename】翻页查看文件，按空格下一页，b 向上翻页， enter 下一行
### less
 * less 【filename】比more多了一个搜索功能，输入"／关键字" ，然后回车
 n 向下查，N 向上查，q 退出，如果希望从文件末尾开始向上查，可以使用"？关键字"

##文件修改和过滤
### echo
 * echo xxx > 【filename】 将xxx写入文件，并覆盖原有内容
 * echo xxx >>【filename】 将xxx写入文件，在文件后面追加
### grep 截取行
 * grep【字符串】【filename】 过滤带有字符串的行
 * grep【^ 字符串】【filename】 过滤以字符串开头的行
 * grep【字符串 $】【filename】 过滤以字符串结尾的行
 * grep -v 【字符串】【filename】 过滤反选
 * grep -i 【字符串】【filename】 不区分大小写过滤带字符串的行
 * grep -C 20【字符串】【filename】查看文件中包含字符串以及上下20行的内容
### cut 截取列
 * cut -d"分隔符" -f20 【filename】 以分隔符来分割，截取第20列
### wc 统计
 * wc 【filename】 统计文件的 行数，单词数，字符数
### sort 排序
 * sort 【filename】默认按照ASCII码首字母排序
 * sort -n -k 2 -t : 【filename】
 将文件以第2列的数字排序，列以：分割
 -n按照数字大小排序，-u剔除重复的行，-r降序排列，-k指定某一列，
 -t 分隔符  
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 