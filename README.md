# GitFlow

# 以下是 github 本仓库的使用说明：
{
	…or create a new repository on the command line
	echo "# GitFlow" >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git remote add origin https://github.com/AzollaGit/GitFlow.git
	git push -u origin master

	…or push an existing repository from the command line
	git remote add origin https://github.com/AzollaGit/GitFlow.git
	git push -u origin master
}

# Git 经验：

1、每次准备提交前，先用 git status 看下，所用文件是不是都 git add 了， 然后再运行提交命令 git commit 

# Git 指令集：

git pull		更新本地仓库的最新改动



git status		检查当前文件状态
git status -s	缩短状态命令的输出

git checkout -b <branch name>		创建分支名，并切换到改分支
git checkout master		切换回主分支

git branch -d <branch name>		删除这个分支


git add <filename>			提交指定文件到->暂存区
git add [file/files/path]
git add -A  				提交所有变化 git add --ALL
git add -u  				提交被修改(modified)和被删除(deleted)文件，不包括新文件(new)
git add .   				提交新文件(new)和被修改(modified)文件，不包括被删除(deleted)文件

git rm <filename>			删除暂存区文件
git rm [file/files/path]	例如 git rm build\*~  删除所有名字以 ~ 结尾的文件
git rm --cached				让文件保留在磁盘，但是并不让 Git 继续跟踪。


git commit -m "代码提交信息"		提交到->HEAD
git commit -a -m "代码提交信息"		跳过 git add 进行提交

git remote add origin <server>		链接远程仓库
git push origin master				推送主分支到远端仓库; 
git push origin <branch name>		推送分支到远端仓库

git diff			查看尚未暂存的文件更新了哪些部分(:q退出)
git diff --staged	查看已暂存的将要添加到下次提交里的内容
git diff --cached 	查看已经暂存起来的变化（ --staged 和 --cached 是同义词）

git log					查看本地仓库的历史记录（q退出）
git log --name-status	查看哪些文件改变了
git log --graph --oneline --decorate --all	通过 ASCII 艺术的树形结构来展示所有的分支, 每个分支都标示了他的名字和标签:


git mv fileOld fileNew	修改 fileOld 文件名 为 fileNew


vim .gitignore		编辑 git 忽略文件
cat .gitignore		查看 git 忽略文件





