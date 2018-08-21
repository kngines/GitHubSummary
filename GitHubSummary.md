# GitHub Summary
**Git 常用命令总结**

 1. 初始化:&nbsp;
    `git init`
 2. 查看当前仓库状态:&nbsp;
    `git status`
 3. 向本地仓库提交文件:&nbsp;
    `git add <file>`
 4. 提交到远程仓库并附加注释:&nbsp;
    `git commit -m 提交注释`
 5. 本地链接远程仓库:&nbsp;
    `git remote add origin repo-address`
 6. 推送到主分支:&nbsp;
    `git push -u origin master` 
 7. 克隆仓库到本地:&nbsp;
    `git clone repo-address` 
 8. 查看提交日志:&nbsp;
    `git log` 
 9. 查看远程仓库版本:&nbsp;
    `git remote -v` 
 10. 删除所有文件:&nbsp;
    `git rm -f *` 
 11. 查看帮助信息:&nbsp;
    `git help config` 
 12. 列出本地分支:&nbsp;
    `git branch` 
 13. 列出远程分支:&nbsp;
    `git branch -r` 
 14. 新建test分支:&nbsp;
    `git branch test` 
 15. 切换到test分支:&nbsp;
    `git checkout test` 
 16. 新建并切换到test分支:&nbsp;
    `git checkout -b test` 
 17. 删除test分支:&nbsp;
    `git branch -d test` 
 18. 强制删除test分支:&nbsp;
    `git branch -D test` 
 19. 获取远程仓库指定分支:&nbsp;
    `git fetch origin branch` 
 20. 推送到远程仓库指定分支:&nbsp;
    `git push origin branch` 
 21. 列出现有标签:&nbsp;
    `git tag` 
 22. 显示指定版本详细信息:&nbsp;
    `git show <version>` 
 23. 全局查询字符串:&nbsp;
    `git grep 查询文本` 
 24. 针对版本查询字符串:&nbsp;
    `git grep 查询文本 v1.0` 
    
---

**创建 GitHub 公钥**
 1. 改变链接方式[HTTP -> SSH]:&nbsp;
    
    `git remote rm origin`
    <br/>`git remote add origin git@github.com:username/respository.git`
 
 2. 创建新的SSH Key:&nbsp;
    
    `cd ~/.ssh`
    <br/>`ssh-keygen`
   
 3. 测试链接（权限拒绝）:&nbsp;
    
    `ssh -T -v git@github.com`
   
 4. 向github添加公钥:&nbsp;
    
    利用 ~/.ssh/id_rsa.pub 内容在 https://github.com/settings/profile 建立 SSH Key.
    
  5. 测试结果
    <br/>`ssh -T git@github.com`
    <br/>提示 : `You've successfully authenticated, but GitHub does not provide shell access.`
    
    