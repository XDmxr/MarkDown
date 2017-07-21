#Git使用指南
##工具

安装 Git for Windows 安装完成后需要配置账户信息
		git config --global user.name "XDmxr"
        git config --global user.email "1303774514@qq.com"
        
安装TortoiseGit，安装选择SSH客户端时选择第二项OpenSSH，Git default SSH Client，其他默认安装。
1. 创建自己的公钥/私钥对： 打开Git Bash -> 输入ssh-keygen -t rsa 其他均回车略过，则会在目录C:\Users\Administrator\.ssh下产生公私钥两个文件 -> 将公钥配置到服务器即可。
2. 将公钥配置到服务器：登录自己的GitHub账户，注意与上面Git的账户信息相同，进入右上角的MyProfile界面，进入SSH Keys 界面，点击 Add new，并点击save保存。公钥会出现在SSH Keys的列表中。到此，通过SSH公钥认证，建立与服务器端的通信完成。

##Git 命令
```      
拉取远程仓库   git pull [remoteName] [localBranchName] 
推送远程仓库   git push [remoteName] [localBranchName]
创建本地分支   git branch [name]注意新分支创建后不会自动切换为当前分支
切换分支      git checkout [name]
创建并立切换为新分支：git checkout -b [name]
删除分支      git branch -d [name] -d选项只能删除已经参与了合并的分支，对于未有合并的分支是无法删				除的。如果想强制删除一个分支，可以使用-D选项
合并分支      git merge[name]  将名称为[name]的分支与当前分支合并


查看版本      git tag
创建远程版本    git push origin [name] 其实是将本地分支push到远程
删除远程版本   git push origin :refs/tags/[name]


## Git提交代码
git add 文件名  -------可以多次使用，添加多个文件
git add .        全部文件
git commit -m “备注内容”
git push origin master


