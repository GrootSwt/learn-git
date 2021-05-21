## 全局设置name和email

```git
git config --global user.name "name"
git config --global user.email "eamail"
```

## 创建空目录

```git
mkdir learn-git
cd learn-git
```

## 将当前目录变成git可管理的仓库

```git
git init
```

## 将文件添加到仓库

```git
// 一次添加一个文件
git add readme.md
// 一次添加多个文件
git add first.txt second.txt
```

## 将文件提交到仓库

```git
git commit -m "新增readme.md文件"
```

## 查看仓库当前状态

```git
git status
```

##  git diff作用

```git
// 查看工作区和缓存区文件不同
git diff readme.md
// 查看缓存区和仓库文件不同
git diff --cached
// 查看工作区和仓库文件不同
git diff HEAD -- readme.md
```

## 查看git提交历史

```git
// 显示全部历史记录
git log
// 显示简略历史记录git 
git log --pretty=online
```

## 版本回退和版本移动

```git
// 版本回退上一个版本
git reset --hard HEAD^
// 版本回退上上版本
git reset --hard HEAD^^
// 版本回退上一百个版本
git reset --hard HEAD~100
// 版本移动（最后为版本号）
git reseet --hard 0b5e04a
```

## 查看每一次版本指向历史记录

```git
git reflog
```

## 从暂存区将文件删除（取消git add操作）

```git
git restore --staged readme.md
```

##  将工作区文件恢复到最新一次提交（也可以用于误删除恢复操作）

```git
git restore readme.md
git chekcout -- readme.md
```

## 从版本库中删除文件

```git
git rm text.txt
git commit -m "删除text.txt"
```

## 创建SSH-key

```git
ssh-keygen -t rsa -C "396518038@qq.com"
```

## 本地仓库关联远程仓库

```git
// origin是远程库的别名
git remote add origin git@github.com:GrootSwt/learn-git.git
```

## 本地库推送远程库

```git
// 本地库和远程库连接后，第一次推送需要加 -u，以后不需要加
git push -u origin master
```

## 取消与远程库的关联

```git
// 查看关联的远程库
git remote -v
// 取消与远程库的关联（根据别名取消关联）
git remote rm origin
```

## 从远程库克隆

```git
git clone git@github.com:GrootSwt/learn-git.git
```

## 创建分支

```git
// 创建dev分支并切换到dev分支
git checkout -b dev
// 创建分支
git branch dev
// 切换分支
git checkout dev
```

## 查看分支

```
git branch
```

## 分支合并

```git
// 指定分支合并到当前分支
git merge dev
```

