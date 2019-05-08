# suanpan-lite
算盘个人版

## 安装 ##
### 前提 ###
windows和mac用户会在安装的过程中安装相应的virtualbox软件

### 安装 ###
#### windows 用户 ####
以管理员权限运行powershell console，执行下面命令
```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
```
从 https://github.com/LuChenjing/suanpan-edu/releases 下载好当前系统匹配的suanpan个人版的压缩包，解压后进入到解压后的目录下面。
目前的版本如下：
```
suanpan-lite-windows.v1.0.*.zip
suanpan-lite-darwin.v1.0.*.tgz
suanpan-lite-linux.v1.0.*.tgz
```
启动算盘
```
./spctl.ps1 start
```
停止算盘
```
./spctl.ps1 stop
```
删除算盘
```
./spctl.ps1 delete
```
查看算盘状态
```
./spctl.ps1 status
```
升级算盘
修改env.ps1中的$env:SP_VERSION="suanpan-edge:2.91.28"，设置为将要升级的版本，执行stop，start


#### Linux 用户 ####
1. 从指定地址下载好Linux版本的suanpan个人版压缩包suanpan-lite-linux.v1.0.*.tgz
比如放到：/home/suanpan/下面
2. 解压这个压缩包
```
tar zxvf suanpan-lite-linux.v1.0.*.tgz -C /home/suanpan
```
3. cd到解压后的目录
```
cd /home/suanpan/suanpan-edu
```

4. 运行spctl.sh（使用root用户执行）
```
sudo su
./spctl start
```
5. 等待终端的log结束显示。


#### mac 用户 ####
1. 解压 suanpan-lite-darwin-v1.0.*.tgz
2. cd到解压后的目录
3. 运行 ./spctl.sh start
3. 如果没有提前安装VirtualBox，程序会自动安装VirtualBox，中途会提示输入sudo密码

