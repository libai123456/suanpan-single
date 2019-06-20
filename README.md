# 算盘个人版使用指南

### 1. 准备安装文件 ###

从如下路径下载好当前系统匹配的算盘个人版的安装文件：

OSS: https://oss.console.aliyun.com/bucket/oss-cn-shanghai/suanpan-public/object

目前的版本如下：
```
Windows: spctl.ps1
Linux/Mac: spctl.sh
```
> 对于windows和mac系统，算盘启动时如果没有检测到virtualbox软件，会在安装的过程中自动安装相应的virtualbox软件，如果系统已经安装了virtualbox软件，算盘将会使用已经安装的virtualbox来启动算盘
> 对于windows系统，算盘启动时会自动下载curl for Windows，用于下载算盘组件。

### 2. 启动算盘 ###

#### windows 用户 ####
1. 将下载下来的算盘安装文件（spctl.ps1）放在一个指定的文件夹下。请保证这个文件夹所在的磁盘至少有超过20g的空间，同时算盘运行会占用
2核cpu以及4G内存。

2. 从开始菜单/搜索中找到 Windows Powershell 程序， 并右键**以管理员权限运行**

3. cd到算盘安装文件所在的目录。

4. 执行下面命令启动算盘
```
./spctl.ps1 start
```

5. 等待启动完成，浏览器自动打开地址 http://splocal.xuelangyun.com:30000

6. 如果使用完毕，需要停止算盘，在安装文件所在文件夹 右键选择stop-suanpan.bat，在上下文菜单中选择**以管理员权限运行**。
如果想要重新启动算盘，在安装文件所在文件夹 右键选择start-suanpan.bat，在上下文菜单中选择**以管理员权限运行**。

7. 如果需要删除算盘，在安装文件所在文件夹 右键选择delete-suanpan.bat，在上下文菜单中选择**以管理员权限运行**。 在停止以后，删除解压目录即可

#### mac 用户 ####
1. 将下载下来的算盘安装文件（spctl.sh）放在一个指定的目录下。请保证这目录所在的磁盘至少有超过20g的空间，同时算盘运行会占用
2核cpu以及4G内存。

2. 打开终端/Terminal， cd到算盘安装文件所在的目录。

3. 执行下面命令启动算盘
```
./spctl.sh start
```

4. 等待启动完成，浏览器自动打开地址 http://splocal.xuelangyun.com:30000

5. 如果使用完毕，需要停止算盘，执行下面命令停止算盘
```
./spctl.sh stop
```
6. 如果需要删除算盘，在停止以后，删除解压目录即可

> 如果没有提前安装VirtualBox，程序会自动安装VirtualBox，中途会提示输入sudo密码

#### Linux 用户 ####
1. 将下载下来的算盘安装文件（spctl.sh）放在一个指定的目录下。请保证至少有超过20g的剩余磁盘空间。

2. cd到算盘安装文件所在的目录。

3. 执行下面命令启动算盘
```
sudo su -
./spctl.sh start
```

4. 等待启动完成，浏览器自动打开地址 http://splocal.xuelangyun.com:30000

5. 如果使用完毕，需要停止算盘，执行下面命令停止算盘
```
sudo su -
./spctl.sh stop
```
6. 如果需要删除算盘，在停止以后，删除解压目录即可

### 3. 设置算盘 ###
在实际使用算盘中，可能会遇到算盘的默认分配的资源（2核cpu，4G内存，20G磁盘）不够的情况。只需要使用工具打开算盘安装文件（spctl.sp1/spctl.sh），修改如下参数即可：
```
Windows: 
$env:MINIKUBE_MEMORY=4000
$env:MINIKUBE_CPUS=2
$env:MINIKUBE_DISK_SIZE="20g"

Linux/Mac: 
export MINIKUBE_MEMORY=4000
export MINIKUBE_CPUS=2
export MINIKUBE_DISK_SIZE=20g
```


