一、git 提交一个project

    $ git init
    $ git remote add origin http://10.128.90.61:18090/ustc_devops/com.hzx.hadoop.spark.git
    $ git config --global user.name "ustc_devops"
    $ git config --global user.email "ustc_devops@163.com"
    $ git add .
    $ git commit -m '集团三码 DevOps 测试'
    $ git push -u origin master
    
二、git 拉去一份新project

    # 第一次可能需要你输入密码
    $ git init .
    $ git remote add origin http://60.174.249.204:48888/CTG-CODEMIX/ngrms-grpcdm.git
    $ git config --global user.name "你的gitlab用户名"
    $ git config --global user.email "你的gitlab邮箱"
    $ git pull origin branch-01
    

三、git 提交文件

    # 这条命令会自己寻找本地修改或创建的文件，也可以指定文件名
    $ git add -A 或者 git add SecondSortLamda.java
    # 说明你提交的内容
    $ git commit -m "二次排序的Lamda表达式实现"
    # git push -u origin HEAD:<name-of-remote-branch> 提交代码到指定的分支
    $ git push -u origin HEAD:Branch-1

四、git clone 代码

    $ git clone http://10.128.90.61:18090/ustc_devops/com.hzx.hadoop.spark.git

五、git 列出所有远程分支

    $ git branch -r

六、切换本地代码，或者检出末次提交到服务器上代码

    # 检出末次提交到服务器上代码 git checkout <tag>
    $ git checkout 9f8b7576abb068dbf303c50334ae29faed40c16b
    # 切换到指定分支 git checkout <name-of-branch>
    $ git checkout Branch-1

七、拉取分支代码

    # git pull origin <name-of-branch> 
    $ git pull origin Branch-1

八、IDEA中git使用

    1、提交代码
    (1)、选中所在工程右键 --> Git --> 单击 Commit Dirctory --> 在 Commit Changes 选中要提交的文件，
    同时填写 Commit Message --> 单击 commit
    (2)、选中所在工程右键 --> Git --> Repository --> 单击 Push --> 在 Push Commits 选择要提交的代码分支
    （自己填写）--> Push

    2、拉取代码
    (1)、选中所在工程右键 --> Git --> Repository --> 单击 Pull --> 在 Pull Changes 选择要拉取代码的分支 --> 单击 Pull