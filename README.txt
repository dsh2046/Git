1. 分支
查看分支：git branch
创建分支：git branch <name>
切换分支：git checkout <name>
创建+切换分支：git checkout -b <name>
合并某分支到当前分支：git merge <name>
删除分支：git branch -d <name>

2. 可视化分支
查看分支合并图： git log --graph --pretty=oneline --abbrev-commit 
(包含时间，用户)： git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
(只包含log，用户名)： git log --pretty=format:'%s %C(bold blue)(%an)%Creset' --abbrev-commit

3. 临时保存当前任务（git stash; git stash pop）
当手头工作没有完成时，先把工作现场git stash一下，然后去修复bug，修复后，再git stash pop，回到工作现场
