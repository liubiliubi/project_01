## 配置指令
```javascript
git config --global user.name "用户名"
git config --global user.email "邮箱地址"

// 查看所有全局配置项
git config --list --global

// 查看特定配置项
git config user.name

// git init 将当前目录转化为Git仓库
git init

// git status -s 以精简的方式显示文件的状态
git status -s 

// git add 有三个功能 ① 可以开始跟踪新文件 ② 把以跟踪的、且以修改的文件放到暂存区 ③ 把有冲突的文件标记为已解决状态
git add

// git add . 将多个文件加入暂存区
git add .

// git commit -m "提交消息" 将暂存区中的文件的快照，提交到Git仓库中进行保存
git commit -m "提交消息"

// git checkout -- 文件名称 撤销对文件的修改 危险系数极高！
git checkout -- 文件名称

// git reset HEAD 要移除的文件名称 将暂存区的文件移除
git reset HEAD .

// git commit -a -m "提交消息" 直接是工作区->Git仓库
git commit -a -m "提交消息"

// git rm -f 文件 从工作区和Git仓库中同时移除对应文件
// git rm --cashed 文件 只移除Git仓库中的对应文件
git rm -f 文件
git rm --cashed

// git log 查看提交历史
git log -2 // 两条

// git log -- pretty=oneline
// git reset --hard <CommitID> 根据ID 回退到指定版本
// git reflog --pretty=oneline 在旧版本中查看命令操作的历史
// git reset --hard <CommitID>
```
## 文件的四种状态

![](2023-09-18-10-11-07.png)