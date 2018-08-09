Git 常用指令
===

## 最基本
```shell
git clone git@<地址>
git add <fileName>
git checkout -- <fileName>
git pull origin <branchName>
git push origin <branchName>
```
## 分支
```shell
# 查看所有的branch
git branch
# 切换分支
git checkout <branchName>
# 创建一个branch并切换过去
git checkout -b <branchName>
# 跟踪远程分支
# git checkout -b <branchName> origin/<branchName>
git fetch origin screenshot:screenshot

# 将本地branch推送到远程仓库
git push origin <branchName>
# 删除本地branch
git branch -D <branchName>
# 删除远程分支
git push origin :master
# 删除远程分支
git push origin --delete master

```
## Git stash保存当前的工作现场
```shell
# 保存工作现场
git stash
# 获取工作现场列表
git stash list
# 恢复工作现场
git stash pop stash@{num}
# 清除工作现场
git stash clear
```
