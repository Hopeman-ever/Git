Git基础使用

用户名和邮箱配置

```
git config --global user.name "用户名"
git config --global user.email "邮箱地址"
```

查询已配置的用户名和邮箱

```
git config --list
```

生成SSH Key:

```
ssh-keygen -t rsa -C "邮箱地址"
```

执行上述命令会在本地c盘生成一个id_rsa.pub文件，以记事本打开改文件，将里面内容拷贝到github的SSH and GPG keys 里面

验证是否成功

```
ssh -T git@github.com
```

![image-20220325200829200](C:\Users\D302\AppData\Roaming\Typora\typora-user-images\image-20220325200829200.png)

建立本地仓库

```
git init
```

指定上传内容

```
git add [file]
```

提交到本地仓库

```
git commit -m '提交说明'
```

指定提交的远程仓库

```
git remote add origin git@github.com:Hopeman-ever/Git.git
```

上传到远程仓库

```
git push origin master
```

