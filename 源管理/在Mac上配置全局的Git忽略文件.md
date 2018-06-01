# 在Mac上配置全局的Git忽略文件

##### 现在同时搞着好几个项目，在Xcode、IDEA、Eclipse之间频繁的切换，每个项目的忽略文件列表都不一样，每个项目都有一个.gitignore，甚是麻烦，今天网上拔出来一个设置全局忽略的办法，记录下来，日后备查。

1. 打开终端：

   ```shell
   1. git config --global core.excludesfile ~/.gitignore_global
   2. vim ~/.gitignore_global
   3. 按i键输入以下内容：
   # for Mac OS X System Files
   .DS_Store
   Thumbs.db
    
   # for emacs
   *~
   [#]*[#]
    
   # for Eclipse
   *.project
    
   # for Logs and databases
   *.log
    
   # remove SVN
   .svn
    
   # for Xcode
   .*.swp
   .clang_complete
   *.xcodeproj/project.xcworkspace/
   *.xcodeproj/xcuserdata/
    
   # for IDEA
   */build/*
   .idea/*
   *.iml
   /out/*
   
   4. 按下esc键输入 ":wq"保存
   ```

