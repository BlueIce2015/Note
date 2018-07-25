### How to use GitHub?

###### 1.new repository

​	uncheck README



###### 2.create a new repository on the command line 

```shell
echo "# TestRepository3" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/username/TestRepository3.gitgit push -u origin master
```

**or push an existing repository from the command line** 

```shell
git init
git config --global user.name "your name"
git config --global user.email "your_email@youremail.com"
可以查看.git/config来确认和修改
git add *
git commit -m "commit text"
git remote add origin git@github.com:BlueIce2015/Note.git
注意这里要使用SSH地址，这样之后的SSH Key才可以正常使用
git push -u origin master
```



###### 3.设置SSH Key，这样在本地客户端就可免输USER/Password

ssh-keygen -t rsa -C "your_email@youremail.com"

后面的`your_email@youremail.com`改为你在github上注册的邮箱，之后会要求确认路径和输入密码，我们这使用默认的一路回车就行。成功的话会在`~/`下生成`.ssh`文件夹，进去，打开`id_rsa.pub`，复制里面的`key`。

回到github上，进入 Account Settings（账户配置），左边选择SSH Keys，Add SSH Key,title随便填，粘贴在你电脑上生成的key。



![beautiful](../../images/still-life.jpg)