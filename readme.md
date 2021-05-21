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



