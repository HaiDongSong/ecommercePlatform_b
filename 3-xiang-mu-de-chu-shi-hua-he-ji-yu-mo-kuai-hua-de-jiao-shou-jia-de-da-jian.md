![](/assets/import30.png)![](/assets/import32.png)

### 1.生成并部署SSH key {#1-ssh-}

你可以按如下命令来生成 sshkey:

```
ssh-keygen -t rsa -C "xxxxx@xxxxx.com"
# Generating public/private rsa key pair...
# 三次回车即可生成 ssh key
```

查看你的 public key，并把他添加到码云（Gitee.com） SSH key添加地址:[https://gitee.com/profile/sshkeys\](https://gitee.com/profile/sshkeys%29\)

```
cat ~/.ssh/id_rsa.pub

# ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC6eNtGpNGwstc....
```

添加后，在终端（Terminal）中输入

```
ssh -T git@gitee.com
```

若返回

```
Welcome 
to
 Gitee.com, yourname!
```

则证明添加成功。

### 2.git使用

```
git clone git@gitee.com:FeiYingZhanDui/mmall-fe.git
//删除下载好的文件夹测试下一个用法

mkdir mmall-fe
cd mmall-fe
git init
touch test.html
git remote add origin git@gitee.com:FeiYingZhanDui/mmall-fe.git
git pull origin master
git status
git add .
git commit -am 'test'(提交并添加注释)
git push
git push --set-upstream origin master
```

这样本地文件夹就和远程仓库连接起来啦，可以刷新仓库看到test.html已经push到仓库中



### 3.项目脚手架的安装

### ![](/assets/import35.png)

### 

### ![](/assets/import36.png)

#### ![](/assets/impor37t.png)官方文档：\[http://webpack.github.io/docs/\]\(http://webpack.github.io/docs/\)

#### 



