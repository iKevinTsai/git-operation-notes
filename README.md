# git-operation-notes
查看分支
```Bash
#本地端
git branch
#遠端
git branch -r
```
新增commit 清單
```Bash
#新增
git add .
#撤銷
git reset
```
建立分支
```Bash
$ git branch develop
$ git checkout develop
#或者
git checkout -b develop
```
Commit 紀錄
```Bash
#本地端
git log
#遠端
git log--oneline
```
從develop開一個 "release"分支並合併至master
```Bash
#目前分支是develop
git checkout -b release
#切換至Master分支
git checkout master
#合併release
git merge release
#給予版本號(會把開一個文字檔案，寫備註)
git tag -a "v0.1"
#刪除release
git branch -d release
git push -u origin master
```
推不上去怎麼辦
```Bash
#方法一:先拉再推
git pull --rebase
#方法二:無敵，蓋就對了
git push -f
```
