## Git 使用

#### Git 与 SVN 区别 

1. GIT是分布式的，SVN不是：这是GIT和其它非分布式的版本控制系统，例如SVN，CVS等，最核心的区别。
2. GIT把内容按元数据方式存储，而SVN是按文件。
3. GIT分支和SVN的分支不同：分支在SVN中一点不特别，就是版本库中的另外的一个目录。
4. GIT没有一个全局的版本号，而SVN有：目前为止这是跟SVN相比GIT缺少的最大的一个特征。
5. GIT的内容完整性要优于SVN：GIT的内容存储使用的是SHA-1哈希算法。这能确保代码内容的完整性，确保在遇到磁盘故障和网络问题时降低对版本库的破坏。

#### Git安装配置

1. 安装包下载地址：<https://gitforwindows.org/>

#### smartGit安装

1. smartGit安装：https://www.syntevo.com/smartgit/download/

2. smartGit破解：

   * windows+R：输入%APPDATA%\syntevo\SmartGit\查找，或直接输入地址在文件夹栏输入![952771-20160927145001860-689017113](https://github.com/lazyAug/notes/blob/master/源管理/images/952771-20160927145001860-689017113.png)

     ![952771-20160927145151547-1113083547](https://github.com/lazyAug/notes/blob/master/源管理/images/952771-20160927145151547-1113083547.png)

   * 找到Setting.xml 的文件夹，把他删掉，重新打开SmartGit 就可以解决序列号的问题了；

   * 安装好客户端以后，就可以使用了

#### smartGit使用

1. 打开SmartGit，在菜单里选择Repository→Clone![20151224093513601](https://github.com/lazyAug/notes/blob/master/源管理/images/20151224093513601.png)
2. 填写Repository URL：这里涛哥或者项目创建者会提供URL
3. 会提示你输入账号密码，这时候输入你在码云网站 https://gitee.com注册的账号密码，以我们公司给到个人企业邮箱来注册。
4. 下一步再下一步，为项目选择一个本地文件夹。![20151224093810427](https://github.com/lazyAug/notes/blob/master/源管理/images/20151224093810427.png)
5. 这里文件名字是自动给你创建好了的，你直接finish就行了，点击Finish，稍等片刻，Output中的信息告诉我们，ok搞定了。
6. 这样你的本地仓库就创建好了。打开你刚刚选择的项目文件夹位置，这里的文件夹就是你的本地仓，这里就是你放文件代码的地方，而 smartgit也是指向这个文件夹的。![20151224095007609](https://github.com/lazyAug/notes/blob/master/源管理/images/20151224095007609.png)
7. 你可以在你的开发工具直接打开这个文件夹进行开发，或者放入你需要提交的文件 ，这样你的文件就自动写入本地仓了。比如我在文件夹下新建了一个txt文件。![20151224101108230](https://github.com/lazyAug/notes/blob/master/源管理/images/20151224101108230.png)
8. 选中你的文件点击commit(提交)，会弹出一个提交框，上面是你的代码文件，下面你写的文件注释 ，然后commit就行，commit后如下图![20151224101432409](https://github.com/lazyAug/notes/blob/master/源管理/images/20151224101432409.png)

![20151224101701412](https://github.com/lazyAug/notes/blob/master/源管理/images/20151224101701412.png)

9. 右侧显示是已经提交成功，这里的提交成功你可以理解为smartgit知道了你要提交的代码，然后你还要看左边的local Branches，
10. master1>origin,这里的">"并不是大于符号，而是指向符号,意思是你还需要你本地的代码提交到网上
11. 选中 master1>origin,单击右键push,就是把你的代码提交到网上

