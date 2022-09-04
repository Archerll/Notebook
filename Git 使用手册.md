# Git 使用手册

## Git的基本概述



## Git的基本命令

`git init`  git 初始化

`git clone` 从仓库克隆一个分支



`git add` 将修改添加到本地仓库

`git mv`

`git restore` 回滚未提交的修改

`git rm` 从本地仓库中删除一个文件



`git bisect`

`git diff`

`git grep`

`git log` 查看日志

`git status`

- 解决 git status 中文乱码问题

git  bash终端键入

```shell
git config --global core.quotepath false
```

`git branch`

`git commit` 

`git merge`

`git reset`





`git fetch`

`git pull`  从master拉取最新的更改

`git push` 将最新的修改推送到master分支



### 配置用户名和邮箱 

配置全局名称```git config --global user.name 'name'```

配置全局emial ```git config --global user.email 'email'```



---

## 如何使用Git同步本地文件到GitHub

新建一个文件夹，在其中添加想要上传的文件

1.执行```git init``` 使用git初始化文件夹，git会自动创建一个master分支

2.执行```git add --all``` 向master分支添加所有文件

3.执行 ```git commit -m "update"``` 将master分支内容进行提交

4.执行```git push git@github.com:Archerll/Notebook.git master ``` 将master分支的内容合并到github的主分支上，这里 “git@github.com:Archerll/Notebook.git”是目标仓库的ssh

这里的第4步也可以使用以下命令：

5.执行```git remote add orign git@github.com:Archerll/Notebook.git```

6.执行```git push -u orign master```



---

## 如何查看修改历史

```git branch``` 查看分支

`git branch --all`   查看全部分支

`git checkout` 

```git status``` 查看

```git log```





