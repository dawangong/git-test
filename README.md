#### git-test
##### git命令

1.本地项目关联到远程仓库
```git
git init
git remote add origin git@github.com:<UserName>/<RepositoriesName>.git
```

2.建立分支
```git
git branch <BranchName>
```

3.切换分支
```git
git checkout <BranchName>
```

4.新建并切换分支
```git
git checkout -b <BranchName>
```

5.查看本地分支
```git
git branch
```

6.查看远程分支
```git
git branch -r
```

7.查看所有分支
```git
git branch -a
```

8.放弃本次修改
```git
git checkout <FileName>
```

9.删除本地分支
```git
git branch -d <BranchName>
```

10.删除远程分支
```git
git push origin --delete <BranchName>
```

11.新建分支push时被动添加关联
```git
git push --set-upstream origin <BranchName>    远程会自动创建同名分支
```

12.新建分支主动push并添加关联
```git
git push -u origin <BranchName>    远程会自动创建同名分支
```

13.推送及拉取指定分支
```git
git push origin <BranchName>
git pull origin <BranchName>
```

14.注释说明写错需要修改时
```git
git commit --amend
```

15.上面指令会进入vm编辑器模式
```git
命令模式下按i进入插入模式修改
ESC键返回命令模式
英文状态下输入 :wq 保存并退出
```

16.英文状态下 按q退出git log

17.合并某分支到当前分支
```git
git merge <BranchName>
```

18.版本回退
```git
git reset --hard HEAD^     回退到上一版本
git reset --hard HEAD^^    回退到上上一版本
git reset --hard HEAD~100  回退到上100版本
git reset --hard <commit id>  回退到某版本
```

19.强制推送
```git
git push -f
git push -f origin <BranchName>
```

20.查看所有分支的所有操作记录（包括（包括commit和reset的操作），包括已经被删除的commit记录
```git
git reflog
```

21.不小心将代码改到了master，想保存改动到qa分支并恢复master
```git
master: git stash
master: git checkout qa
qa: git stash apply
```

22.基本
```git
git add .            添加所有改动文件到缓存区
git commit -m "xxx"  提交修改
git push             当前分支只有一个远程分支时
git clone <https> | <ssh>
```


