### cocoapods安装使用

#### 安装or升级Ruby

1. 在 .bash_profile 文件中加入“source ~/.profile”语句

2. 打开终端：输入 

   ```shell
   1. ls -a
   2. open .bash_profile
   
   //在文件里写入：
   export PATH=/usr/local/bin:$PATH
   source ~/.profile
   //保存关闭文件
   ```

3. 安装rvm

   ```shell
   1. curl -L https://get.rvm.io | bash -s stable
   2. source ~/.bashrc
   3. source ~/.bash_profile
   4. rvm -v
   ```

4. 列出已知的ruby版本，安装需要的版本

   ```shell
   1. rvm list known
   2. rvm install 2.4
   ```

5. 等待下载完成，编译完成以后，Ruby, Ruby Gems 就安装好了。

6. 查询已安装的ruby版本，卸载一个已安装版本

   ```shell
   1. rvm list
   2. rvm remove 2.0.0
   ```

7. RVM 装好以后，需要执行下面的命令将指定版本的 Ruby 设置为系统默认版本

   ```shell
   rvm 2.0.0 –default 
   ```

#### Ruby更换源

```shell
gem source -r https://rubygems.org/  
gem source -a https://gems.ruby-china.org/
gem sources -l
```

#### cocoaPods安装

1. 如果之前装过cocopods，最好先卸载掉，卸载命令：

   ```shell
   1. sudo gem uninstall cocoapods【Mac 10.10之前】
   2. sudo gem uninstall -n /usr/local/bin cocoapods【Mac 10.11之后】
   3. gem list --local | grep cocoapods
   //会显示如下：
   cocoapods-core (0.39.0)
   cocoapods-downloader (0.9.3)
   cocoapods-plugins (0.4.2)
   cocoapods-search (0.1.0)
   cocoapods-stats (0.6.2)
   cocoapods-trunk (0.6.4)
   cocoapods-try (0.5.1)
   
   然后逐个删除吧：
   sudo gem uninstall cocoapods-core【Mac 10.10之前】
   sudo gem uninstall -n /usr/local/bin cocoapods-core【Mac 10.11之后】
   ```

2. 下载安装cocoaPods

   ```shell
   1. sudo gem install -n /usr/local/bin cocoapods
   2. pod setup
   ```

   

   

    