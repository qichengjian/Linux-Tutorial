##用户和组相关的文件
### ／etc／passwd
每一行都代表一个账号，有几行就代表有几个账号

系统账号：bin，daemon，adm，nobody
### ／etc／shadow
存放密码及其策略相关的信息

### ／etc／group
存放用户组的信息

### ／etc／gshadow
存放用户组的密码及其策略相关的信息

##用户和组的相关命令
### 新建用户和组
#### groupadd 创建组 -g 指定gid，-r 创建的是系统组
 * groupadd -g 888 test  新建组test，指定组id为888
 * groupadd -r baby    新建一个系统组baby
#### ueradd 创建用户

### 用户身份切换 sudo su
 * su 【username】切换用户
 
 * sudo -u 【username】【command】 以用户权限执行命令
 


