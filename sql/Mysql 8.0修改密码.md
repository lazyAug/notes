### Mysql 8.0修改密码

1. mysql -u root -p '原来的密码'   //进入数据库中

2. show databases；

3. use mysql；

4. 使用下面的语句修改密码：

   ```sql
   ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '你的密码';
   ```

5. 推出，使用新的密码登陆

