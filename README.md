## GitHubTips
### GitHub开发常用

- 配置用户信息
	
		git config --global user.name "kngines"
		git config --global user.email "kngines@163.com"

- 开启SSH服务
	
		apt-get install ssh # Ubuntu 安装 SSH
		yum install ssh 	# CentOS 安装 SSH
		ps -e | grep sshd 	# 查看 SSH 服务状态

- 生成 SSH Key
	
		ssh-keygen -t rsa -C "kngines@163.com"

- 克隆仓库到本地

		git clone git@github.com:kngines/jupyter-analysis-ipynb.git

- 向本地仓库提交文件

		git add .

- 提交到远程仓库并附加注释

		git commit -m "update some files"

- 推送到主分支

		git push -u origin master

		git push git@github.com:kngines/jupyter-analysis-ipynb.git

- 添加远程仓库

		git remote add origin git@github.com:username/respository.git


- 测试成功

		ssh -T git@github.com # 提示 : `You've successfully authenticated, but GitHub does not provide shell access.

- 查看git全局配置
	
		git config --global -e

- 配置ss代理. 通过socks5协议走ss通道
		
		git config --global http.proxy 'socks5://127.0.0.1:1080'
		git config --global https.proxy 'socks5://127.0.0.1:1080'

- 取消ss代理配置

		git config --global --unset http.proxy
		git config --global --unset https.proxy

### Github基础命令
- 初始化
   
      git init
 
- 查看当前仓库状态
  
      git status
	
- 向本地仓库提交文件
 	
      git add <file>
	
- 提交到远程仓库并附加注释
 	
      git commit -m 提交注释
	
- 本地链接远程仓库
 	
      git remote add origin repo-address
	
- 推送到主分支
 	
      git push -u origin master
	
- 克隆仓库到本地

      git clone repo-address
	
- 查看提交日志

      git log
	
- 查看远程仓库版本

      git remote -v

- 删除所有文件

      git rm -f *
	
- 查看帮助信息

      git help config	
	
- 列出本地分支

      git branch	
	
- 列出远程分支

      git branch -r	
	
- 新建test分支

      git branch test	
	
- 切换到test分支

      git checkout test	
	
- 新建并切换到test分支

      git checkout -b test
	
- 删除test分支

      git branch -d test
	
- 强制删除test分支

      git branch -D test	
	
- 获取远程仓库指定分支

      git fetch origin branch	
	
- 推送到远程仓库指定分支

      git push origin branch	
	
- 列出现有标签

      git tag		 
	
- 显示指定版本详细信息

      git show <version>	
	
- 全局查询字符串

      git grep 查询文本	
	
- 针对版本查询字符串

      git grep 查询文本 v1.0	
		
