一文学懂Git，原来Git这么强大！
Git作为程序员必备技巧之一！这是你需要了解的知识点。
本次笔记阅读渠道有
公众号推文：[https://mp.weixin.qq.com/s?__biz=MzkwMTIyMzg5MQ==&mid=2247484212&idx=1&sn=84c22a7efc8f3b9bd14d9b59efc3aa99&chksm=c0b94788f7cece9efc9d786c9d98ab507943dc2e3c6bcece207bc1914925936867de3fe6f0ae#rd](https://mp.weixin.qq.com/s?__biz=MzkwMTIyMzg5MQ==&mid=2247484212&idx=1&sn=84c22a7efc8f3b9bd14d9b59efc3aa99&chksm=c0b94788f7cece9efc9d786c9d98ab507943dc2e3c6bcece207bc1914925936867de3fe6f0ae#rd)
Github南城余笔记仓库：
CSDN:
大家好，我是南城余！今天给大家分享下Git的再学习，本次学习弥补了之前不太懂Git原理以及其他git命令了解，给大家贴上了我学习的网站链接，以供我写的不清楚的时候，大家可以翻阅。
> https://pdai.tech/md/devops/tool/tool-git.html
> https://www.runoob.com/git/git-tutorial.html（菜鸟教程）
> https://zhuanlan.zhihu.com/p/193140870（知乎）

### 什么是git?为什么要学习？
Git 是一个开源的分布式版本控制系统，用于敏捷高效地处理任何或小或大的项目。
作为一个程序员，git是必备的，因为你需要将你的代码托管到代码仓库，可以很好的管理你的代码版本，遇到bug回退代码版本，虽然现在的编译器也支持代码历史记录，但依然抵触不了，代码仓库是个好东西。
主流代码仓库有
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694745777049-416803bb-a0e6-4500-bfca-b9eb83e14197.png#averageHue=%23fcfcfb&clientId=u0d302199-122f-4&from=paste&height=410&id=u785d0aae&originHeight=461&originWidth=895&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=18526&status=done&style=none&taskId=u1dd703fd-beb8-4c24-8a08-44c8a906a70&title=&width=795.5555555555555)
并且作为程序员，我们要有开源精神，帮助互联网时代共建美好未来
可以看下面csdn文章链接开源精神
[https://blog.csdn.net/phena/article/details/109635639](https://blog.csdn.net/phena/article/details/109635639)
不管是什么开发工具，其实都有可视化操作工具
例如数据库有navicat，redis有Another Redis Desktop Manager，所以git也不例外。
如果你实在不想敲命令，可以下载git可视化管理工具
参考链接：
[https://www.runoob.com/git/source-tree-intro.html](https://www.runoob.com/git/source-tree-intro.html)


### 代码提交和同步代码
#### 架构图
![](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694679751467-d28c986d-f58a-48d9-bea0-df6d4af3a98a.png#averageHue=%23f2eee3&clientId=u02170bb9-e56a-4&from=paste&id=u1853caa8&originHeight=518&originWidth=1139&originalType=url&ratio=1.125&rotation=0&showTitle=false&status=done&style=none&taskId=udb278fd1-058e-4941-9395-8e99022da8d&title=)
#### Git操作代码提交和同步代码-常用操作命令
第0步：工作区与仓库保持一致
```git
git status
```
第1步：文件增删改，变为已修改状态
第2步：git add ，变为已暂存状态
```git
git add --all #当前项目下的所以更改 
git add . #当前目录下的所有更改
git add xx/xx.py xx/xx2.py #添加其中几个文件
```
第3步：git commit,变为已提交状态
```git
git commit -m "这里写此次提交的描述" 
```
第4步：git push,变为已推送状态
```git
git push -u origin master #第一次需要关联分支
git push #之后推送就不用指明应该提交的远程分支了
git branch #可以查看本地仓库分支
git branch -a #可以查看本地仓库和远程仓库的所有分支
```

#### 实操演示
实操参考链接（知乎）：
[https://zhuanlan.zhihu.com/p/193140870](https://zhuanlan.zhihu.com/p/193140870)
来源TechmindWave项目
链接：[https://mp.weixin.qq.com/s/FlzCd4PqOReqxszU6Nfw_g](https://mp.weixin.qq.com/s/FlzCd4PqOReqxszU6Nfw_g)
##### 1）在GitHub上创建仓库


![](https://cdn.nlark.com/yuque/0/2023/png/38420467/1692242894607-117b277f-4f70-467c-9ba8-a759e8787307.png?x-oss-process=image%2Fresize%2Cw_843%2Climit_0#averageHue=%23625347&from=url&id=zFZMU&originHeight=384&originWidth=843&originalType=binary&ratio=1.125&rotation=0&showTitle=false&status=done&style=none&title=)

![](https://cdn.nlark.com/yuque/0/2023/png/38420467/1692243009840-75d03b0d-a569-4da8-879b-3a40e8fbff95.png#averageHue=%23e8ebc2&from=url&id=apFnE&originHeight=833&originWidth=1793&originalType=binary&ratio=1.125&rotation=0&showTitle=false&status=done&style=none&title=)
创建成功后，你可能用到的命令

2）建立本地仓库

![](https://cdn.nlark.com/yuque/0/2023/png/38420467/1692243278870-bf82f194-3176-41b5-aab8-444ab462455e.png?x-oss-process=image%2Fresize%2Cw_784%2Climit_0#averageHue=%23f3f2f1&from=url&id=miQ1F&originHeight=837&originWidth=784&originalType=binary&ratio=1.125&rotation=0&showTitle=false&status=done&style=none&title=)
进入git命令台

![](https://cdn.nlark.com/yuque/0/2023/png/38420467/1692243317002-234e8e5f-c735-4183-8892-8ca7c94eaa9d.png#averageHue=%230a0a0a&from=url&id=BVtaC&originHeight=460&originWidth=736&originalType=binary&ratio=1.125&rotation=0&showTitle=false&status=done&style=none&title=)
输入git init,初始化项目
##### 3） 将所有文件添加到仓库中
```git
git add . 
```
##### 4）修改文件描述
```git
git commit-m "first commit"
```
##### 5）关联github仓库
```git
git branch-M main
git remote add origingit@github.com:nanchengcyu/TechMindWave-frontend.git #改为自己的
```
##### 6）上传本地代码
```git
git push -u origin main
```


### 代码撤销和撤销同步
#### 架构图
![](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694679805685-2aa36a60-3539-4da1-b1b7-35a4b18e5c66.png#averageHue=%23f4f2ef&clientId=u02170bb9-e56a-4&from=paste&id=ud7247c7e&originHeight=543&originWidth=1141&originalType=url&ratio=1.125&rotation=0&showTitle=false&status=done&style=none&taskId=uad2b4bc6-f4b6-40c9-a4f7-0a1e0dce3d6&title=)
#### Git常用操作命令 - 代码撤销和撤销同步
##### 已修改，但未暂存
```git
git diff #列出所有的修改
git diff xx/xx.py #列出指定文件修改
git checkout #撤销项目下的所有修改
git checkout .#撤销当前文件夹下的所有修改
git clean -f # untracked状态，撤销新增的文件
git clean -df # untracked状态，撤销新增的文件和文件夹

```
#### 已暂存，未提交
> 这个时候已经执行过git add，但未执行git commit，但是用git diff已经看不到任何修改。 因为git diff检查的是工作区与暂存区之间的差异。

```bash
$ git diff --cached # 这个命令显示暂存区和本地仓库的差异

$ git reset # 暂存区的修改恢复到工作区
$ git reset --soft # 与git reset等价，回到已修改状态，修改的内容仍然在工作区中
$ git reset --hard # 回到未修改状态，清空暂存区和工作区
```
git reset --hard 操作等价于 git reset 和 git checkout 2步操作
#### 已提交，未推送
> 执行完commit之后，会在仓库中生成一个版本号(hash值)，标志这次提交。之后任何时候，都可以借助这个hash值回退到这次提交。

```bash
$ git diff <branch-name1> <branch-name2> # 比较2个分支之间的差异
$ git diff master origin/master # 查看本地仓库与本地远程仓库的差异

$ git reset --hard origin/master # 回退与本地远程仓库一致
$ git reset --hard HEAD^ # 回退到本地仓库上一个版本
$ git reset --hard <hash code> # 回退到任意版本
$ git reset --soft/git reset # 回退且回到已修改状态，修改仍保留在工作区中。
```
#### [#](#已推送到远程) 已推送到远程
```java
$ git push -f orgin master # 强制覆盖远程分支
$ git push -f # 如果之前已经用 -u 关联过，则可省略分支名
```
> 慎用，一般情况下，本地分支比远程要新，所以可以直接推送到远程，但有时推送到远程后发现有问题，进行了版本回退，旧版本或者分叉版本推送到远程，需要添加 -f参数，表示强制覆盖。



拉取仓库代码到本地
参考链接：
[https://blog.csdn.net/soulerge/article/details/118972737](https://blog.csdn.net/soulerge/article/details/118972737)
```git
git clone https链接
```
### Git常用命令
git clone、git push、git add 、git commit、git checkout、git pull
参考代码含义
[**https://www.runoob.com/git/git-basic-operations.html**](https://www.runoob.com/git/git-basic-operations.html)

### Git二次上传多次上传方法
[https://blog.csdn.net/weixin_50492082/article/details/108777018](https://blog.csdn.net/weixin_50492082/article/details/108777018)

