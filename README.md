# 算盘个人版使用指南

### 1. 准备安装包 ###

从如下路径下载好当前系统匹配的算盘个人版的安装包：
OSS: https://oss.console.aliyun.com/bucket/oss-cn-shanghai/suanpan-public/object
Github: https://github.com/LuChenjing/suanpan-edu/releases 

目前的版本如下：
```
suanpan-lite-windows.v1.0.*.zip
suanpan-lite-darwin.v1.0.*.tgz
suanpan-lite-linux.v1.0.*.tgz
```
> 对于windows和mac系统，算盘启动时如果没有检测到virtualbox软件，会在安装的过程中自动安装相应的virtualbox软件，如果系统已经安装了virtualbox软件，算盘将会使用已经安装的virtualbox来启动算盘

### 2. 启动算盘 ###

#### windows 用户 ####
1. 解压suanpan-lite-windows-v1.0.*.zip安装包

2. 右键选择start-suanpan.bat，在上下文菜单中选择**以管理员权限运行**

3. 等待启动完成，浏览器自动打开地址 http://splocal.xuelangyun.com:30000

4. 如果使用完毕，需要停止算盘，右键选择stop-suanpan.bat，在上下文菜单中选择**以管理员权限运行**

5. 如果需要删除算盘，在停止以后，删除解压目录即可

#### mac 用户 ####
1. 解压suanpan-lite-darwin-v1.0.*.tgz
```
tar zxvf suanpan-lite-darwin.v1.0.*.tgz
```
2. cd到解压后的目录

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
1. 解压suanpan-lite-linux.v1.0.*.tgz
```
tar zxvf suanpan-lite-linux.v1.0.*.tgz
```
2. cd到解压后的目录

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



