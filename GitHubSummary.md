# GitHub Summary
**Git 常用命令总结**

 1. 初始化
     `git init`
 2. 查看当前仓库状态
    `git status`
 3. 向本地仓库提交文件
    `git add <file>`
 4. 提交到远程仓库并附加注释
    `git commit -m 提交注释`
 5. 本地链接远程仓库
    `git remote add origin repo-address`
 6. 推送到主分支
    `git push -u origin master` 
 7. 克隆仓库到本地
    `git clone repo-address` 
 8. 查看提交日志
    `git log` 
 9. 查看远程仓库版本
    `git remote -v` 
 10. 删除所有文件
    `git rm -f *` 
 11. 查看帮助信息
    `git help config` 
 12. 列出本地分支
    `git branch` 
 13. 列出远程分支
    `git branch -r` 
 14. 新建test分支
    `git branch test` 
 15. 切换到test分支
    `git checkout test` 
 16. 新建并切换到test分支
    `git checkout -b test` 
 17. 删除test分支
    `git branch -d test` 
 18. 强制删除test分支
    `git branch -D test` 
 19. 获取远程仓库指定分支
    `git fetch origin branch` 
 20. 推送到远程仓库指定分支
    `git push origin branch` 
 21. 列出现有标签
    `git tag` 
 22. 显示指定版本详细信息
    `git show <version>` 
 23. 全局查询字符串
    `git grep 查询文本` 
 24. 针对版本查询字符串
    `git grep 查询文本 v1.0` 