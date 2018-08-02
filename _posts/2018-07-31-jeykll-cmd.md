```
$ git add .

$ git commit -m "some commit message"

$ git push origin master

```
Git 提交时提示 "The file will have its original line endings in your working directory", 在 Git 中输入如下命令解决：
````git config --global core.autocrlf false````