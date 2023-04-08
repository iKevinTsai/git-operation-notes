如何建立新的branch
```Bash
#切換到你要基於哪一個分支來建立分支，如master
git checkout origin master
#拉最新的版本
git pull
#開始建立新branch
git branch develop
#切換新branch
git checkout develop
#push to remote
git push -u origin develop
```
