# 一、基础知识
相关链接：[https://www.runoob.com/linux/](https://www.runoob.com/linux/)

![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1690965466530-ddf76d8b-dec8-4cf5-8236-19015d6e4924.png#averageHue=%23f9f0ef&clientId=ufa7ad0b8-5d43-4&from=paste&height=500&id=ucc13235b&originHeight=2531&originWidth=1170&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=555755&status=done&style=none&taskId=u1ec47899-3a10-46bd-b20c-9bd192d0c7c&title=&width=231)
## 1.1Linux软连接和硬链接
相关链接：[https://zhuanlan.zhihu.com/p/67366919](https://zhuanlan.zhihu.com/p/67366919)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1691572357236-2c16a920-4436-4040-a44c-e9e5c1d0a73b.png#averageHue=%23f5f2f0&clientId=u6be2d933-ac3c-4&from=paste&height=468&id=ucc701454&originHeight=526&originWidth=875&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=73528&status=done&style=none&taskId=uec0e4310-3738-4922-8365-85b88d5e123&title=&width=777.7777777777778)
## 1.2Linux 系统启动过程
相关链接：[https://www.runoob.com/linux/linux-system-boot.html](https://www.runoob.com/linux/linux-system-boot.html)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1691717581788-e99d1a20-2c35-436f-92e4-84c9e5d33c94.png#averageHue=%23f8f8f7&clientId=u0e655aa2-93f4-4&from=paste&height=524&id=uc15f7439&originHeight=589&originWidth=1111&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=58320&status=done&style=none&taskId=u31e9c429-caa9-463e-86a0-b9fca51590a&title=&width=987.5555555555555)
# 二、小知识点总结
## 2.1重启或或者关闭系统时，先执行 sync将内存中的数据同步到磁盘中。
相关连接：[https://www.runoob.com/linux/linux-system-boot.html](https://www.runoob.com/linux/linux-system-boot.html)
关机指令：shutdown  重启指令：reboot
## 2.2目录
./表示当前目录  ../表示上一层目录![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1691725215951-6d87ccc6-8e95-4d4f-837c-8ba01a01a1a0.png#averageHue=%23faf9f9&clientId=u0e655aa2-93f4-4&from=paste&height=132&id=ufaed95f1&originHeight=149&originWidth=1041&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=17483&status=done&style=none&taskId=ubfdb809e-21a5-453b-ab82-4af9a1b7773&title=&width=925.3333333333334)![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1691725246840-ed9dd512-0370-4cbc-910a-47152777eb4e.png#averageHue=%23fbfaf9&clientId=u0e655aa2-93f4-4&from=paste&height=128&id=uc94f35ac&originHeight=144&originWidth=1076&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=15681&status=done&style=none&taskId=u07d16a92-715c-4b4a-b97b-c303846155b&title=&width=956.4444444444445)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1691725592405-f37bb6b7-3dc0-461b-ae39-c933978b9afc.png#averageHue=%23f0f0f0&clientId=u0e655aa2-93f4-4&from=paste&height=301&id=u585eec31&originHeight=339&originWidth=969&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=52261&status=done&style=none&taskId=uc79bfbe7-4478-4674-8ee6-0e9d1ae6906&title=&width=861.3333333333334)
### 文件颜色表示
```
   白色：表示普通文件
   蓝色：表示目录
   绿色：表示可执行文件
   红色：表示压缩文件
   浅蓝色：链接文件
   红色闪烁：表示链接的文件有问题
   黄色：表示设备文件
   灰色：表示其它文件
```
### 目录总结
**系统启动必须：**

- **/boot：**存放的启动Linux 时使用的内核文件，包括连接文件以及镜像文件。
- **/etc：**存放**所有**的系统需要的**配置文件**和**子目录列表，**更改目录下的文件可能会导致系统不能启动。
- **/lib**：存放基本代码库（比如c++库），其作用类似于Windows里的DLL文件。几乎所有的应用程序都需要用到这些共享库。
- **/sys**： 这是linux2.6内核的一个很大的变化。该目录下安装了2.6内核中新出现的一个文件系统 sysfs 。sysfs文件系统集成了下面3种文件系统的信息：针对进程信息的proc文件系统、针对设备的devfs文件系统以及针对伪终端的devpts文件系统。该文件系统是内核设备树的一个直观反映。当一个内核对象被创建的时候，对应的文件和目录也在内核对象子系统中

**指令集合：**

- **/bin：**存放着最常用的程序和指令
- **/sbin：**只有系统管理员能使用的程序和指令。

**外部文件管理：**

- **/dev ：**Device(设备)的缩写, 存放的是Linux的外部设备。**注意：**在Linux中访问设备和访问文件的方式是相同的。
- **/media**：类windows的**其他设备，**例如U盘、光驱等等，识别后linux会把设备放到这个目录下。
- **/mnt**：临时挂载别的文件系统的，我们可以将光驱挂载在/mnt/上，然后进入该目录就可以查看光驱里的内容了。

**临时文件：**

- **/run**：是一个临时文件系统，存储系统启动以来的信息。当系统重启时，这个目录下的文件应该被删掉或清除。如果你的系统上有 /var/run 目录，应该让它指向 run。
- **/lost+found**：一般情况下为空的，系统非法关机后，这里就存放一些文件。
- **/tmp**：这个目录是用来存放一些临时文件的。

**账户：**

- **/root**：系统管理员的用户主目录。
- **/home**：用户的主目录，以用户的账号命名的。
- **/usr**：用户的很多应用程序和文件都放在这个目录下，类似于windows下的program files目录。
- **/usr/bin：**系统用户使用的应用程序与指令。
- **/usr/sbin：**超级用户使用的比较高级的管理程序和系统守护程序。
- **/usr/src：**内核源代码默认的放置目录。

**运行过程中要用：**

- **/var**：存放经常修改的数据，比如程序运行的日志文件（/var/log 目录下）。
- **/proc**：管理**内存空间！**虚拟的目录，是系统内存的映射，我们可以直接访问这个目录来，获取系统信息。这个目录的内容不在硬盘上而是在内存里，我们也可以直接修改里面的某些文件来做修改。

**扩展用的：**

- **/opt**：默认是空的，我们安装额外软件可以放在这个里面。
- **/srv**：存放服务启动后需要提取的数据**（不用服务器就是空）**
## 2.3文件基本属性
chown（change owner）:修改所属用户与组   更改文件属主 属组 
chgrp 更改文件属组
上面语法
chown/chgrp [-R] 属主名/属组名  文件名
chmod (change mode):修改用户的权限
ll或者ls -l 查询之后 
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1691736646339-9ec01375-62d8-4e16-b061-8f5e8b71d740.png#averageHue=%2329495e&clientId=ud1eea726-802d-4&from=paste&height=307&id=u56ed4d1a&originHeight=345&originWidth=509&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=280091&status=done&style=none&taskId=u5e821e74-ab7f-4d8c-b34d-8ffcfc4356e&title=&width=452.44444444444446)
开头字母为d是目录
开头字母为-是文件
开头字母为l表示为链接文档（硬链接和软连接）
开头字母为b表示装置文件里面的可供储存的接口设备（可随机存取装置)）
开头字母为c表示装置文件里面的串行端口设备（键盘、鼠标）
后面连续字母每三个一组 字母意思分别为 r-可读 w-可写 r-可执行 

![](https://cdn.nlark.com/yuque/0/2023/jpeg/38420467/1691738206667-e4a44c3b-acdb-4adc-be3b-1b65318c0d5c.jpeg)
## 2.4 文件与目录管理
### 2.4.1路径
./表示当前目录  ../表示上一层目录
绝对路径：路径由根目录/写起 例如：/usr/share/doc
相对路径：路径的写法，不由/写起 例如由 /usr/share/doc 要到 /usr/share/man 底下时，可以写成： **cd ../man** 这就是相对路径的写法。
# 三、相关指令
## 3.1清屏指令
相关远程应用如finalshell、xshell等均可
```powershell
(1)CTRL+l 或者 CTRL+k
(2)直接命令输入clear
```
## 3.2 进入/root目录下
```powershell
cd ~
```
## 3.3 进入顶级目录 /
```powershell
cd /
```
# 四、shell
## 4.1运行shell脚本
### 4.1.1作为可执行程序
将上面的代码保存为test.sh ,并cd到相应目录下
```powershell
chmod +x .test.sh #chmod是脚本具有执行权限 x(execute)
./test.sh #执行脚本
```
### 4.1.2作为解释器参数
直接运行解释器，其参数就是 shell 脚本的文件名
```powershell
/bin/sh test.sh
/bin/php test.php
```
## 4.2shell知识扩展
### 4.2.1什么是shell
Shell 是一个用 C 语言编写的程序，它是用户使用 Linux 的桥梁。Shell 既是一种命令语言，又是一种程序设计语言。
Shell 是指一种应用程序，这个应用程序提供了一个界面，用户通过这个界面访问操作系统内核的服务。
Ken Thompson 的 sh 是第一种 Unix Shell，**Windows Explorer** 是一个典型的图形界面 Shell。
**Windows Explorer** 
知识链接：
[https://www.zhihu.com/question/310462143](https://www.zhihu.com/question/310462143)
## 4.3shell脚本编程
shell脚本在线运行网站：
[https://www.runoob.com/try/showbash.php?filename=helloworld](https://www.runoob.com/try/showbash.php?filename=helloworld)
```shell
my_name="nanchengyu\n"
hello="my name is ${my_name}"
echo $myname $hello
```
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1692609181922-87381435-3f63-43a4-8e5e-342157fd0caa.png#averageHue=%23fdfdfd&clientId=u69bef78c-6f7c-4&from=paste&height=512&id=u6ad0246a&originHeight=576&originWidth=1879&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=43978&status=done&style=none&taskId=u1554e9d6-f5a9-4f50-8863-1fbecc2c9f5&title=&width=1670.2222222222222)
## 4.4运维常用命令
网站地址：[https://zhuanlan.zhihu.com/p/36093355](https://zhuanlan.zhihu.com/p/36093355)
### 4.4.1查看端口命令
```bash
netstat -tuln

```
-t 表示列出 TCP 端口，-u 表示列出 UDP 端口，-l 表示仅列出监听端口，-n 表示以数字形式显示地址和端口。
```bash
lsof -i :端口号
```
    
将 "端口号" 替换为你想要查看的具体端口号。
### 4.4.2 运行jar包命令
```bash
java -jar 文件名.jar
```
```bash
java -jar 文件名.jar --spring.profiles.active=prod
```

### 4.4.3 ps命令
```bash
ps -vref |grep java
```
这条命令的作用是查找正在运行的 Java 进程，并显示详细的进程信息。其中：

- ps: 显示当前进程的状态。
- -v: 显示详细信息。
- -r: 按照进程的 PID 排序。
- -f: 显示完整格式的进程信息。
- |: 管道符号，将前一个命令的输出作为后一个命令的输入。
- grep: 文本搜索工具，用于在输入中查找包含指定字符串的行。
- java: 要搜索的字符串，这里是 Java 进程。
### 4.4.4 docker容器相关指令
```bash
docker ps -a
```
```bash
docker start redis
```
# 基本指令学习
## cat
查看文本内容、文件行数、字符数、单词数等 
合并文本内容
## chattr
改变文件属性
## chgrp
用于改变文件、目录所属群组
## chmod
控制用户对文件权限的命令


