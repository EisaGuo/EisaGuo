- 👋 Hi, I’m @EisaGuo
- 👀 I’m interested in computer science
- 🌱 I’m currently learning how to use GitHub

2024-10-21
BV1Cr4y1J7iQ
Introduction to Git
  VCS: version control system--help us to manage our coding
  After downloading Git, open the second choice: Git Bash Here 控制台
  click program, options, text, select, Consolas
  $ git config -- global user.name Eisa
  $ git config -- global user.email trump@bukaopu.com

  有两种初始化方式
  git clone: using coding from GitHub
    GitHub, code, cone, HTTPS, copy link
    $git clone (paste the link) 然后回车
    桌面上就会出现项目文件夹, 打开有个.git文件夹, 大部分文件最好别去操作
  git init: managing our coding
    自己新建文件夹作为自己项目的总文件夹, 进入文件夹打开git bash here
    $git init
    然后开始写代码, 代码所在的目录，叫做工作区, 在工作区新建源代码文件
    main.py
    右击, Edit with IDLE, 假装完成了一个小项目, 然后commit到git作为备份
    但是不要直接操作.git这个文件夹, commit是通过两个命令实现的
    这个 . 是当前文件夹的意思, 告诉git把当前工作台除了.git文件的文件都准备上传
    $git add .
    $git commit -m"XXX此次上传的备注部分（功能1已经完成）"
    以后可以用$git log来查看提交的历史记录

    如果发现自己工作台中的代码文件被小屁孩修改了, 可以用checkout命令进行恢复
    $git checkout HEAD main.py
    会把main.py复制到工作区（会覆盖）
    再次打开源代码，发现昨天的内容回来了

    如果我们在main.py完成了项目2，但是正在兴头上，另外开了一个3.py写项目3，把功能3完成了一半
    有一个问题：如果按照上次的方式$git add .则会把文件夹下所有的文件都提交，这样并不好，因为功能3只完成了一半，我们每次提交的代码应该是清晰的
    则把.换成main.py，备注完成项目2
    $git add main.py
    $git commit -m "功能2完成“

    等到功能3也完成的时候，我们再把3.py子弹上膛
    $git add 3.py
    $git commit -m "功能3完成"

    我们每次都用两步步骤，第一步，把工作区的文档，放到暂存区，名字叫做index or stage
    这个暂存区不是必须的，有些版本控制软件version control system，例如SVN，就没有暂存区，直接把源文件从工作区提交到仓库

  Summary: Git, download, clone, init, commit, checkout, 工作区，暂存区，仓库
  更多内容，看官方出品免费电子书：pro git
  我的建议还是去好好玩几遍 https://learngitbranching.js.org/?locale=zh_CN git 游戏, 理解一下 git 的底层逻辑
  不然以后你碰到 git 问题真的挺恶心的. 如果你真的把版本控制弄的一团糟, https://ohshitgit.com/ 是你的解药.
    
    

