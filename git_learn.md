# git learning

## 1. git diff 学习
git diff          -> 对比暂存区和工作区，显示已修改未暂存内容；
git diff --staged -> 对比版本库和暂存区， 显示已暂存未提交内容
git diff --cached 等同于 --statged
## 2. git rm 学习
rm xx.x + git rm xx.x -> 移除已跟踪文件，不再纳入版本管理
git rm -f xx.x        -> 删除已修改或已暂存文件
git rm --cached xx.x  -> 从版本库和暂存区中删除文件，但保留在工作区

## 3. git mv 学习
git mv xx.x xx1.x  -> 改名子

## 3. git log 学习

## 4. git comit 

*git commit --amend* -> 处理“提交完发现忘记暂存某些修改”或“修改提交信息 

## 5. git remote

git remote  show orgin      -> 查看远程仓库的详细信息 
git remote rename origin pb -> 将远程仓库名字orgin改为pb
git remote remove           -> 移除远程仓库

## 6. 撤销操作
git reset HEAD a.xx  -> 取消a文件的暂存
git checkout -- a.xx -> 取消a文件的修改

## 7. git tag
git tag aaa -> 创建标签aaa
git show || git tag    -> 显示标签
git tag -d aaa         -> 删除标签
git tag bbb hash_value -> 后期补打标签
git push --tags        -> 将标签推送到远程仓, 没有--tags只会保留在本地
git checkout aaa       -> 切换至指定标签版本 

## 8. git push 
git push -f orgin master -> 强制推送到远程仓（可用于版本回退）
