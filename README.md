# shiyanlou-code
这是在实验楼学习Git、Python的笔记
# 将GitHub远程仓库与本地仓库关联起来
* 方法一：在本地新建一个人与远程仓库同名的文件夹

`git init`

将新建的文件夹设置为Git仓库

添加文件,比如我们新写了一个hello.txt：

`git add hello.txt`

`git commit -m "first commit"`

到此为止已经提交到了本地仓库

接下来我们把本地仓库和远程仓库联系起来

`git remote add origin 仓库`

添加后，远程库的名字就是origin，这是Git默认的叫法，也可以改成别的，但是origin这个名字一看就知道是远程库

下一步，就可以把本地库的所有内容推送到远程库上

`git push -u origin master`

由于远程库是空的，我们第一次推送master分支时，加上了-u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令不用-u。


* 方法二：使用Git clone直接从远程仓库克隆下来。先创建远程库，然后，从远程库克隆

`git clone`
不仅仅是自己的仓库可以克隆，也可以克隆其他用户的公开仓库。
## git命令
`git add 文件名`

`git commit -m "first commit"`

`git push origin master`
