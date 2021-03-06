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

文章标题就直接是文件标题，如果文件是以```2018-08-05-考拉是坏蛋.md```命名，那网站上最终显示的文章标题就是```考拉是坏蛋```。但是如果在文章头部加入以下语法，那不管文件是怎么命名的，文章标题就可以自定义了。

```
---
title: 文章题目
---
```

注意，不管加没加上面的语法，网站上文章的链接一定会显示文件名字。所以文件最好用英文命名，这样在复制粘贴时会保留英文的文件名，如果是中文命名的文件，那复制链接时会失去中文的名字。