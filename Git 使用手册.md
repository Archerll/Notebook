# Git 使用手册

## Git的基本概述

## Git的基本命令

### 配置用户名和邮箱

配置全局名称```git config --global user.name 'name'```

配置全局emial ```git config --global user.email 'email'```

## 如何使用Git同步本地文件到GitHub

新建一个文件夹，在其中添加想要上传的文件

1.执行```git init``` 使用git初始化文件夹，git会自动创建一个master分支

2.执行```git add --all``` 向master分支添加所有文件

3.执行 ```git commit -m "update"``` 将master分支内容进行提交

4.执行```git push git@github.com:Archerll/Notebook.git master ``` 将master分支的内容合并到github的主分支上，这里 “git@github.com:Archerll/Notebook.git”是目标仓库的ssh

这里的第4步也可以使用以下命令：

5.执行```git remote add orign git@github.com:Archerll/Notebook.git```

6.执行```git push -u orign master```



## 如何查看修改历史

```git branch```

```git status```

```git log```





