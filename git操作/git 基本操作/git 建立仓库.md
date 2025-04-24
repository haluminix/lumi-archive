从本地已有项目建立远程仓库



1、跳转到项目目录下

```bash
git init
```

2、新建一个远程同名（好像可以不同名，但是最好同名）仓库

3、执行以下命令

```bash
git remote add origin git@github.com:gitname/reponame.git
```

4、查看是否添加成功

```bash
git remote -v
```

如果成功可以看到下面的输出

```
origin  git@github.com:xxxx.git (fetch)
origin  git@github.com:xxxx.git (push)
```

5、添加本地文件并提交

```bash
git add .
git commit -m "初始化项目"
```

6、推送到远程

把本地分支重命名为 main（如果你的 GitHub 仓库默认是 main）

```bash
git branch -M main  
```

 把代码推送到 GitHub

```bash
git push -u origin main 
```

