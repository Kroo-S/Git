

git remote set-url origin  https://<your_token>@github.com/<USERNAME>/<REPO>.git



# 一、git基本信息
    1. git status       查看git当前状态

    2. git init         初始化git项目

    3. git config       git配置相关操作
        3.1. 查看git当前所有配置的位置
             git config --list --show-origin      
        3.2. 设置用户信息
            git config --global user.name "XXX"
            git config --global user.email xxx@XX.com

    4. git help  查看git命令行使用方法
        4.1. git help status
        4.2. git status --help

    5. Q：退出

=======================================================

    
# 二、git提交代码

【基本流程】 修改文件 -》 暂存区 -》 提交更新

    git init 初始化
    git status 查看git状态
    git add .   提交所有git代码（后面加一个点）  提交到暂存区
    git commit -m "feat:project init"   提交到本地数据库中
    git log 查看刚刚提交的版本信息
    git diff 比较文件的差异化

=======================================================

# 三、Git协作：如何分支管理

    git branch feature/3-4       创建分支   </br>
    
    git checkout feature/3-4     切换到新建的分支   </br>
    
    git merge feature/3-4        合并分支

【 上传到github 】
1. github上创建仓库
2. 关联本地仓库
    git remote add origin https://github.com/<USERNAME>/<REPO>.git
    git push -u origin main    上传
    git pull origin master     将远程仓库的代码拉取到本地


=======================================================

# 四、Token

1. 通过指令修改密码为token
git config user.password "<your_token>"

2. 把token直接添加远程仓库链接中，这样就可以避免同一个仓库每次提交代码都要输入token

git remote set-url origin  https://<your_token>@github.com/<USERNAME>/<REPO>.git

<your_token>:换成你自己得到的token
<USERNAME>:你自己的GitHub的用户名
<REPO>:你自己的仓库名称

=======================================================

# 五、VSCode相关问题

Q1:VSCode提交代码后，一直转：

https://blog.csdn.net/Er_Studying_Bai/article/details/128088429?ops_request_misc=&request_id=&biz_id=102&utm_term=vscode上传github代码，提交后一直加载&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-0-128088429.142^v87^control_2,239^v2^insert_chatgpt&spm=1018.2226.3001.4187


Q2:VSCode代码提交

https://www.bilibili.com/video/BV1dK411p7RF/?spm_id_from=333.337.search-card.all.click&vd_source=6ffa2e348a638cae44b435eff005e657

=====================================================================

# 六、Github用户名更改

https://blog.csdn.net/weixin_44285445/article/details/107833418?ops_request_misc=&request_id=&biz_id=102&utm_term=github%E7%94%A8%E6%88%B7%E5%90%8D%E6%9B%B4%E6%94%B9&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-0-107833418.142^v87^insert_down28,239^v2^insert_chatgpt&spm=1018.2226.3001.4187
