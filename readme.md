# 全局设置name和email

```git
git config --global user.name "name"
git config --global user.email "eamail"
```

# 创建版本库

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

```
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

