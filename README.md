算盘个人版安装

windows 用户
1. 解压 suanpan-lite-windows-v1.0.*.zip
2. 管理员权限运行 powershell console
3. cd到解压后的目录
4. 执行 Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
5. 运行 ./spctl.ps1 start
6. 如果没有提前安装VirtualBox，程序会自动安装，有可能会有一次重启，两台机器测试，有一台重启了，具体原因在查。
7. 如果碰到了重启，需要回到目录再运行./spctl.ps1 start，程序会检测到VirtualBox已经装好，不会再装，会直接部署

Linux 用户
1. 解压 suanpan-lite-linux.v1.0.*.tgz
2. cd到解压后的目录
3. 运行 ./spctl.sh start（使用root用户执行）

mac 用户
1. 解压 suanpan-lite-darwin-v1.0.*.tgz
2. cd到解压后的目录
3. 运行 ./spctl.sh start
3. 如果没有提前安装VirtualBox，程序会自动安装VirtualBox，中途会提示输入sudo密码

