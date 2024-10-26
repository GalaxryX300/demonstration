# 如何维护wiki并做贡献

## Github

### 什么是GitHub？

GitHub 是一个基于 Git 的代码托管平台，广泛用于软件开发和版本控制。它提供了一个协作环境，使开发者能够在全球范围内共享和管理代码。以下是 GitHub 的一些关键功能和特点：

1. **版本控制**：利用 Git 的分布式版本控制系统，开发者可以跟踪代码的更改历史，轻松管理项目的不同版本。
2. **协作工具**：通过 pull requests、issues 和 project boards，团队可以高效地进行代码审查、任务分配和项目管理。
3. **代码托管**：GitHub 提供免费的公共仓库和付费的私有仓库存储，支持多种编程语言的项目。
4. **社区和开源**：GitHub 是开源项目的热门平台，开发者可以贡献代码、报告问题和参与讨论。
5. **集成和扩展**：支持与 CI/CD 工具、项目管理软件和其他开发工具的集成，增强了开发流程的自动化和效率。
6. **GitHub Actions**：允许开发者创建自定义的自动化工作流，以实现持续集成和部署。
7. **安全性**：提供代码扫描、依赖项管理和安全警报，帮助开发者识别和修复潜在的安全漏洞。

GitHub 不仅是一个代码托管平台，也是一个开发者社区，促进了全球范围内的协作和创新。

### 如何使用GitHub

[从零开始使用Github Desktop在Github上贡献源代码](https://sdnuroboticsailab.github.io/resource/software/Git/e3-github-contribution/)

## Git

Git 是目前世界上最先进的分布式版本控制系统，用来团队协作很方便。

 如何安装看这个👇

[Git 的安装教程（详解每个步骤）_git官网安装-CSDN博客](https://blog.csdn.net/Passerby_Wang/article/details/120767020?ops_request_misc=%7B%22request%5Fid%22%3A%22169673342216800182730025%22%2C%22scm%22%3A%2220140713.130102334..%22%7D&request_id=169673342216800182730025&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-4-120767020-null-null.142^v95^chatgptT3_1&utm_term=安装git&spm=1018.2226.3001.4187)

配置git环境：git config --global
参数讲解：

> config：参数是用来配置git环境的
>
> --global：长命令表示配置整个git环境

初次使用git需要设置你的用户名以及邮箱，这将作为当前机器git的标识，如果你用它来下载远程仓库一些需要登录权限的仓库会要求登录，git默认使用配置邮箱以及用户名登入，但会要求你手动输入密码

用户名配置

`user`代表用户，`.name`代表配置用户的名称

`git config --global user.name "你的用户名"`
邮箱配置

> user代表用户，.email代表配置用户的邮箱

`git config --global user.email "你的邮箱"`

但是我们基本不会再git bash里敲git命令，要么是在IDE里点点点，要么是在IDE的命令行里敲

如何使用看这个👇

[Git版本控制及Goland使用Git教程_goland配置git-CSDN博客](https://blog.csdn.net/qq_42956653/article/details/121613703?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_utm_term~default-5-121613703-blog-123849753.235^v43^pc_blog_bottom_relevance_base6&spm=1001.2101.3001.4242.4&utm_relevant_index=8)

实验室Wiki目前有比较完善的Git教程。👇

[第一章：什么是Git - SDNU机器人与人工智能实验室](https://sdnuroboticsailab.github.io/resource/software/Git/a1-what-is-git/)

## Git 和 GitHub 如何协同工作？

将文件上传到 GitHub 时，会将其存储在“Git 存储库”中。 这意味着，对 GitHub 中的文件进行更改（或“提交”）时，Git 会自动开始跟踪和管理更改。

可在浏览器中直接在 GitHub 上完成大量与 Git 相关的操作，例如创建 Git 存储库、创建分支以及上传和编辑文件。

但是，大多数人在本地（在自己的计算机上）处理文件，然后不断地将这些本地更改（以及所有相关的 Git 数据）与 GitHub 上的中央“远程”存储库进行同步。 有许多工具可执行此操作，比如 GitHub Desktop。

开始与其他人的协作后，所有人都需要同时在同一存储库上工作，你将不断：

- 从 GitHub 上的远程存储库“拉取”协作者所做的所有最新更改。
- 将你自己的更改“推送”回 GitHub 上的同一远程存储库。

Git 负责确定如何智能地合并此更改流，GitHub 可通过“拉取请求”等功能帮助你管理更改流。

## 从哪里开始？

如果你刚开始使用 GitHub，并且不熟悉 Git，我们建议阅读“[开始你的旅程](https://docs.github.com/zh/get-started/start-your-journey)”类别中的文章。 这些文章重点介绍可以直接在浏览器中在 GitHub 上完成的任务，并帮助你：

- 在 GitHub 上“创建帐户”。
- 了解“GitHub 流程”，以及协作式工作的主要原理（分支、提交、拉取请求、合并）。
- **个性化个人资料**以分享你的兴趣和技能。
- **浏览 GitHub** 以找到自己的项目的灵感，并与其他人联系。
- 了解如何**下载**感兴趣的代码供自己使用。
- 了解如何将正在处理的内容**上传**到 GitHub 存储库。

## Git学习

### 基本 Git 命令

为使用 Git，开发人员使用特定命令来复制、创建、更改和合并代码。 这些命令可以直接从命令行执行，也可以使用 GitHub Desktop等应用程序执行。 以下是使用 Git 的一些常用命令：

- `git init` 初始化一个全新的 Git 存储库并开始跟踪现有目录。 它在现有目录中添加一个隐藏的子文件夹，该子文件夹包含版本控制所需的内部数据结构。
- `git clone` 创建远程已存在的项目的本地副本。 克隆包括项目的所有文件、历史记录和分支。
- `git add` 暂存更改。 Git 跟踪对开发人员代码库的更改，但有必要暂存更改并拍摄更改的快照，以将其包含在项目的历史记录中。 此命令执行暂存，即该两步过程的第一部分。 暂存的任何更改都将成为下一个快照的一部分，并成为项目历史记录的一部分。 通过单独暂存和提交，开发人员可以完全控制其项目的历史记录，而无需更改其编码和工作方式。
- `git commit` 将快照保存到项目历史记录中并完成更改跟踪过程。 简言之，提交就像拍照一样。 任何使用 `git add` 暂存的内容都将成为使用 `git commit` 的快照的一部分。
- `git status` 将更改的状态显示为未跟踪、已修改或已暂存。
- `git branch` 显示正在本地处理的分支。
- `git merge` 将开发线合并在一起。 此命令通常用于合并在两个不同分支上所做的更改。 例如，当开发人员想要将功能分支中的更改合并到主分支以进行部署时，他们会合并。
- `git pull` 使用远程对应项的更新来更新本地开发线。 如果队友已向远程上的分支进行了提交，并且他们希望将这些更改反映到其本地环境中，则开发人员将使用此命令。
- `git push` 使用本地对分支所做的任何提交来更新远程存储库

<img src="C:\Users\evil angle\AppData\Roaming\Typora\typora-user-images\image-20241021195706387.png" alt="image-20241021195706387" style="zoom: 67%;" />

#### 示例：参与现有存储库

```bash
解释# download a repository on GitHub to our machine
# Replace `owner/repo` with the owner and name of the repository to clone
git clone https://github.com/owner/repo.git
 
# change into the `repo` directory
cd repo
 
# create a new branch to store any new changes
git branch my-branch
 
# switch to that branch (line of development)
git checkout my-branch
 
# make changes, for example, edit `file1.md` and `file2.md` using the text editor
 
# stage the changed files
git add file1.md file2.md
 
# take a snapshot of the staging area (anything that's been added)
git commit -m "my snapshot"
 
# push changes to github
git push --set-upstream origin my-branch
```

#### 示例：启动新存储库并将其发布到

首先，您需要在 GitHub 上创建一个新存储库。 有关详细信息，请参阅“[Hello World](https://docs.github.com/zh/get-started/start-your-journey/hello-world)”。 不要使用 README、.gitignore 或 License 文件初始化存储库。 这个空存储库将等待您的代码。

```bash
解释# create a new directory, and initialize it with git-specific functions
git init my-repo
 
# change into the `my-repo` directory
cd my-repo
 
# create the first file in the project
touch README.md
 
# git isn't aware of the file, stage it
git add README.md
 
# take a snapshot of the staging area
git commit -m "add README to initial commit"
 
# provide the path for the repository you created on github
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY-NAME.git
 
# push changes to github
git push --set-upstream origin main
```

#### 示例：为 GitHub 的现有分支做出贡献

此示例假定计算机上已有一个名为 `repo` 的项目，并且自上次在本地进行更改以来，已将新分支推送到 GitHub。

```bash
解释# change into the `repo` directory
cd repo
 
# update all remote tracking branches, and the currently checked out branch
git pull
 
# change into the existing branch called `feature-a`
git checkout feature-a
 
# make changes, for example, edit `file1.md` using the text editor
 
# stage the changed file
git add file1.md
 
# take a snapshot of the staging area
git commit -m "edit file1"
 
# push changes to github
git push
```

## GitHub 的使用

### 1.1 watch、star、fork

### **watch**

watch翻译过来可以称之为观察，点击watch可以看到如下的列表。

默认每一个用户都是处于Not watching的状态，当你选择Watching，表示你以后会关注这个项目的所有动态，以后只要这个项目发生变动，如被别人提交了pull request、被别人发起了issue等等情况，

你都会在自己的个人通知中心，收到一条通知消息，如果你设置了个人邮箱，那么你的邮箱也可能收到相应的邮件。那么以后任何人只要在这个项目下提交了 issue 或者在 issue 下面有任何留言，我的通知中心就会通知我。如果你配置了邮箱，你还可能会因此不断的收到邮件。

### star

star 翻译过来应该是星星，但是这个翻译没任何具体意义，这里解释为`关注`或者`点赞`更合适，当你点击 star,表示你喜欢这个项目或者通俗点，可以把他理解成朋友圈的点赞吧，表示对这个项目的支持。

不过相比朋友圈的点赞，github 里面会有一个列表，专门收集了你所有 start 过的项目，

点击 github 个人头像，可以看到 your star的条目，点击就可以查看你 star 过的所有项目了。

### fork

当选择 fork，相当于你自己有了一份原项目的拷贝，当然这个拷贝只是针对当时的项目文件，如果后续原项目文件发生改变，你必须通过其他的方式去同步。

一般来说，我们不需要使用 fork 这个功能，除非有一些项目，可能存在 bug 或者可以继续优化的地方，你想帮助原项目作者去完善这个项目或者单纯的想在原来项目基础上己维护一个属于自己项目（比如我 fork 的 [AndroidWeekly 客户端](https://link.jianshu.com/?t=https%3A%2F%2Fgithub.com%2Fmaoruibin%2FAndroidWeekly)，那么你可以 fork 一份项目下来，然后自己对这个项目进行修改完善，当你觉得项目没问题了，你就可以尝试发起 pull request 给原项目作者了。

然后就静静等待他的 merge 邮件通知了。

![image-20241026012213992](C:\Users\evil angle\AppData\Roaming\Typora\typora-user-images\image-20241026012213992.png)

### 1.2 获取资源的方式

首先先找到自己需要的项目，然后点击绿色**Code**

![image-20240622163401916](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013143212_image-20240622163401916.png)

可以看到有三种下载方式

![image-20240622163437379](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013143321_image-20240622163437379.png)

1. 使用你的Idea或者pycharm使用HTTPS代码直接爬取
2. 使用你电脑上自带的Github来下载
3. 使用压缩包下载

### 1.2 GitHub项目创建

先来到右上角找到这个加号，并点击

![image-20240622163705811](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013143457_image-20240622163705811.png)

点击New repository，即可新建一个项目

![image-20240622163738906](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013143529_image-20240622163738906.png)

1. 项目名称
2. 项目介绍（中英文均可）
3. 创建一个README文件（**建议勾选**）

![image-20240622164043846]https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013143618_image-20240622164043846.png)

点击绿色按钮**“Create repository**创建项目

![image-20240622164130199](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013143704_image-20240622164130199.png)

创建好后的界面

![image-20240622164223598](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013143806_image-20240622164223598.png)

### 1.3 互动功能

找到**Issues**按钮点击

![image-20240622164312304](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144003_image-20240622164312304.png)

点解绿色**“New issue”**按钮创建新的话题、议题、问题等意思

![image-20240622164459573](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013143909_image-20240622164459573.png)

1. 写标题
2. 写内容

![image-20240622164802072](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144041_image-20240622164802072.png)

随后点击绿色按钮**“Submit new issue”**即可

### 1.4 使用git将项目上传上去：

[Github配置ssh key的步骤（大白话+包含原理解释）_github生成ssh key-CSDN博客](https://blog.csdn.net/weixin_42310154/article/details/118340458)

#### 1.4.1 生成ssh key

首先要检查是否已经生成密钥，可以查看自己的电脑，位置在C:\Users\Username\ .ssh里面，

![image-20241013215319563](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144120_image-20241013215319563.png)

如果没有，可以通过 ssh-keygen-t rsa -C "自己的邮箱"来生成（直接一路回车就好，因为没有截图，就直接用网图了）

![image-20241013215451136](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144159_image-20241013215451136.png)

生成之后去上面的位置点开id_rsa.pub（可用记事本打开），得到ssh key公钥

![image-20241013215553516](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144231_image-20241013215553516.png)

#### 1.4.2 为GitHub配置ssh key

复制之后去GitHub官网，点击右上角头像并找到设置

![image-20241013215629021](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144304_image-20241013215629021.png)

随后点击左侧的SSH and GPG keys，并点击绿色的**New SSH key**

![image-20241013215743120](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144356_image-20241013215743120.png)

![image-20241013215836317](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144430_image-20241013215836317.png)

随便写一个这个ssh连接的名字（红色箭头），将你上面复制的id_rsa.pub文件中key粘贴到下面框中（蓝色箭头）点击**Add SSH key**就可以了。上图就是添加成功的图。

![image-20241013215923123](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144506_image-20241013215923123.png)

#### 1.4.3 建立本地仓库

```text
git init //把这个目录变成Git可以管理的仓库
git add README.md //文件添加到仓库
git add . //不但可以跟单一文件，还可以跟通配符，更可以跟目录。一个点就把当前目录下所有未追踪的文件全部add了 
git commit -m "first commit" //把文件提交到仓库
git remote add origin git@github.com:wangjiax9/practice.git //关联远程仓库
git push -u origin master（这里的master要看，有时候这里不同你要换） //把本地库的所有内容推送到远程库上
```

然后先变成git可以管理的仓库

![image-20241013220236278](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144546_image-20241013220236278.png)

然后你会发现你的文件夹中多了一个.git文件

**注意：**这个目录是Git用来跟踪管理版本库的，没事千万不要手动修改这个目录里面的文件，不然改乱了，就把Git仓库给破坏了。

![image-20241013220523065](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144620_image-20241013220523065.png)

随后将文件添加到仓库：git add （文件名）/git add .（我这里是之后截的图）

![image-20241013220426883](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144709_image-20241013220426883.png)

随后把文件提交到仓库，双引号内是提交注释。使用命令git commit -m "提交信息"

![image-20241013220706084](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144742_image-20241013220706084.png)

这样本地仓库就建立好了。

#### 1.4.4 关联GitHub仓库

到自己的GitHub项目下复制仓库连接

![image-20241013220900084](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144814_image-20241013220900084.png)

随后执行命令：git remote add origin git@github.com:1zero0/PlantVSZombies.git

![image-20241013220946332](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013144848_image-20241013220946332.png)

可以使用git remote -v查看自己的连接（我这里使用的是http的）

![image-20241013221128560](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013145038_image-20241013221128560.png)

#### 1.4.5 上传本地项目

执行命令：git push -u origin main（这里main可能不同）

![image-20241013221203920](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013145142_image-20241013221203920.png)

随后就可以去自己的项目下面看了，已经上传成功了。

![image-20241013221231090](https://images.cnblogs.com/cnblogs_com/blogs/729264/galleries/2425820/o_241013145215_image-20241013221231090.png)

## Typora

### 什么是markdown？

Markdown是一门标记语言。假如你们知道HTML的话，Markdown和HTML可以认为是同类事物。简而言之，就是用纯文本的代码描述带格式文本的一种方法。

那么有了HTML，要Markdown有何用？最简单的答案是：HTML太难写了！

这样对于关注内容的作者而言友好了很多，而且即使是Markdown代码也有相当强的可读性。

于是写好Markdown后，如何将其显示成我们想要的格式呢？通常的做法是将Markdown编译为HTML。其实一些网站已经自带了这样的编译器，输入Markdown代码后直接将其转化为HTML，就可以交给浏览器渲染了。GitHub上的README以及各种.md格式文件的预览功能就是最典型的例子。

Markdown 编写的文档后缀为 `.md`, `.markdown`

### 什么地方会用到markdown？

Markdown可以广泛用于文档、博客、论坛等带格式文本内容的创作，习惯后使用起来会比所见即所得的HTML编辑器更加方便快捷，较Word等格式又有纯文本这一优势。

### typora又是啥

而 typora 就是一款非常方便的支持 md 格式的笔记软件，有很多功能：实时预览、数学公式、代码高亮、表格、支持HTML、流程图等等

这份文档就是在 typora 里敲出来的，个人认为比 word 好用多了

官网下载就完事了https://typora.io/    （看到购买通知可以无视，一直试用就好了

学习版：
[Windows（不要更新）](https://ed.qcea.top/ChaIndex/Softwares/Windows/Editor/Markdown/Typora/typora_64bit_v1.8.10_setup.zip)
[Win/Mac/Linux](https://blog.tcea.top/posts/20231001-typora-crack/)

### Markdown 基本语法及排版规范

[Markdown 基本语法 | Markdown 教程](https://markdown.com.cn/basic-syntax/)

[开源观察贡献指南：Markdown 排版指北 - FOSScope](https://fosscope.com/wiki/fosscope-workflow/markdown-format-guidelines)