# how to use git from basics

[Git] Fork 한 repository 최신으로 동기화하기
ref: https://json.postype.com/post/210431

```
git remote -v
git remote add upstream  
git remote -v
```
## github.com/lge-ros2/cloud_bridge 로 부터 최신걸로 가져옴
```
git fetch upstream
```
## 원하는 local master branch 로 변경
```
git checkout dashing
```

## local branch 에 머지
```
git merge upstream/dashing
```

## lcoal 소스를 github.com/swgu931/cloud_bridge 에 push
```
git push origin dashing
```




##git overwrite update, 강제 업데이트 하기
- https://integer-ji.tistory.com/242?category=745989

```
git reset --hard
git pull
```
```
git commit --amend --reset-author
```
```
git add *
git commit -m "..."
git push origin HEAD:refs/for/develop
```
