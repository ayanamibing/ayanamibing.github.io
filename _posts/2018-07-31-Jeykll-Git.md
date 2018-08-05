---
title: 一些 Jekyll 问题
cover_url: https://i.loli.net/2018/08/02/5b6328902cfb3.jpg
---
Git 提交时提示
 "The file will have its original line endings in your working directory"
在 Git 中输入如下命令解决：
```git config --global core.autocrlf false```

用 Git 发布博客的几个命令：
```
$ git add .

$ git commit -m "some commit message"

$ git push origin master
```

如果远程端（GitHub）有更改，那就需要先把远程的文件先拉下来再 push，使用命令：
```
$ git pull origin master
```