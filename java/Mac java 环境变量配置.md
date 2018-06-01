### Mac java 环境变量配置

1. 在终端输入  /usr/libexec/java_home  可以得到JAVA_HOME 的路径

2. 另外开一个终端，输入 sudo vim /etc/profile 

3. 输入如下配置：

   ```java
   JAVA_HOME="1.得到的路径"
   export JAVA_HOME
   CLASS_PATH="$JAVA_HOME/lib"
   PATH=".$PATH:$JAVA_HOME/bin"
   ```

4. 按ESC，进入保存，输入  :wq!   保存

5. 输入 source /etc/profile

6. 检查环境。输入 echo $JAVA_HOME

   得到配置的路径，说明配置完毕。