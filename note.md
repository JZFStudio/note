# 项目开发中遇到的问题

* vue开发过程中使用vuex时报错state of undefined

    > 在注册store后，需要挂载new Vue下面即可
    
* Mac中忘记mysql密码重

    1. 关闭服务
    2. 进入终端输入：cd /usr/local/mysql/bin/
       回车后 登录管理员权限 sudo su
       回车后输入以下命令来禁止mysql验证功能 ./mysqld_safe --skip-grant-tables &
       回车后mysql会自动重启（偏好设置中mysql的状态会变成running）    

    2. 输入命令 ./mysql
       回车后，输入命令 FLUSH PRIVILEGES;
       回车后，输入命令 SET PASSWORD FOR 'root'@'localhost' = PASSWORD('你的新密码');

