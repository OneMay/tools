linux 使用
=========================================
## 文件

- /usr 最庞大的目录，因为所有应用程序几乎都安装在这里， 本地安装的程序和其他东西在/usr/local 下。
- /usr/bin 几乎所有用户命令.有些命令在/bin 或/usr/local/bin 中
- /usr/src 存放程序的源代码，linux内核的源代码存放在/usr/src/kernels。
- /var 包括系统一般运行时要改变的数据.每个系统是特定的，即不通过网络与其他计算机共享
- /etc： 这个目录相当重要，如前所述，你的开机与系统数据文件均在这个目录之下，因此当这个目录被破坏，那你的系统大概也就差不多该死掉了！而在往后的文件中，你 会发现我们常常使用这个目录下的 /etc/rc.d/init.d 这个子目录，因为这个 init.d 子目录是开启一些 Linux 系统服务的 scripts （可以想成是批次档 ）的地方。而在 /etc/rc.d/rc.local 这个文件是开机的执行档。
- /home：这个是系统将有账号的人口的家目录设置的地方
## 常用命令

- df -h  :查看硬盘空间
- fdisk -l 可查看有没有数据盘（ 没有/dev/vdb，则无数据盘，无需分区挂载）
- mkdir  : 创建文件夹
- rm -rf /var/log/httpd/access  :文件删除
- -r 就是向下递归，不管有多少级目录，一并删除
- -f 就是直接强行删除，不作任何提示的意思
- apt-get install mongodb :安装mongodb
- sudo apt-get --purge remove mongodb mongodb-clients mongodb-server :卸载MongoDB
- unzip wwwroot.zip :解压  wwwroot.zip