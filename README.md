# 算盘个人版使用指南

## 安装 ##
### 前提 ###
对于windows和mac系统，算盘启动时如果没有检测到virtualbox软件，会在安装的过程中自动安装相应的virtualbox软件

从 https://github.com/LuChenjing/suanpan-edu/releases 下载好当前系统匹配的算盘个人版的安装包
目前的版本如下：
```
suanpan-lite-windows.v1.0.*.zip
suanpan-lite-darwin.v1.0.*.tgz
suanpan-lite-linux.v1.0.*.tgz
```

#### windows 用户 ####
1. 解压suanpan-lite-windows-v1.0.x安装包

2. 右键选择start-suanpan.bat，在上下文菜单中选择**以管理员权限运行**

3. 等待启动完成，浏览器自动打开地址 http://splocal.xuelangyun.com:30000

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



