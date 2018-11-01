git i a distributed version control system.
git is free software distributed under the GPL.
git has a mutable index called stage.
git dif
git diff --cached
1 fix bug 101
git tracks changes of files.
first git push origin master.
creating a new brach is quick.
creating a new branch is quick and simple.
git stash fix bug
创建远程分支：
git checkout -b dev
git push origin dev
Git clone非master分支的代码
git branch -r #查看远程分支
git branch -a  #查看所有分支
复制远程分支的方法：
方法1：	git checkout origin/dev   #直接就将远程分支clone下来了
	注意通过上面的方法clone出来的分支是一个游离分支，需要合并到工作分支如dev分支
	方法是：  git branch temp   git checkout dev     git merge temp
方法2：
	git fetch origin dev:temp   #在本地新建一个temp分支，并将远程origin仓库的master分支代码下载到本地temp分支
	git checkout dev      git merge temp   git branch -d temp
推送分支到远程
git push origin dev