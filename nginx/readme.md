nginx 使用
=========================================

## 常用命令

- systemctl restart nginx.service  启动服务 //service nginx restart  //ngix
- nginx -s stop 停止 
- nginx -s reload #重载配置文件
- netstat -apn | grep :80  查看80端口是否被占用
- fuser 80/tcp  kill掉
-  ps -ef|grep nginx  kill –QUIT nginx的master进程号
- kill -9 进程号 暴力停止