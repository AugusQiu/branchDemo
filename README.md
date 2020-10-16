# branchDemo
主分支、标签管理
## 主分支管理常见命令
````
git branch  //查看当前分支
git branch -a   //查看所有分支(包括本地分支、远程分支)
git checkout -b dev remotes/origin/dev  //拉取远程分支到本地，本地分支取名dev
git branch -vv //查看本地和远程分支的关联性

git checkout -b test //直接新建本地分支
git push origin test //推送远程分支
git branch --set-upstream-to=origin/test   //关联本地和远程分支
````
## 打标签常见命令
每次commit的时候，可以给当前推送打上标签  
[掘金git标签讲解](https://juejin.im/post/6844903961770590221)
````
git add .
git commit -m'feat:打标签'
git tag -a v1.0 -m'发布新版本1.0' // 添加附注标签
git show [tagName]
git push origin tagName //推送时，只是push无法成功，需后跟标签名
git log
````
## 合并分支
````
git checkout master //切回主支
git merge dev       //合并分支
git status          //查看状态
````
