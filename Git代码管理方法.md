## 上传本地代码至GitHub
1. github上创建Repository。
2. 新建仓库目录Test
```
git init
```
3. 将项目中所有文件添加到仓库
```
git add .
```
4. 添加文件
```
git add README.md
```
5. 提交到仓库
```
git commit -m '注释语句'
```
6. 将本地仓库关联到github
```
git remote add origin https://github.com/kenlab-chung/vue.js.git
```
7. 上传github之前pull一下
```
git pull origin master
```
8. 上传代码到github远程仓库
```
git push -u origin master
```

## 更新代码至GitHub
1. 查看当前git库状态
```
git status
git diff
```
2. 更新全部
```
git add *
```
3. 提交
```
git commit -m "更新说明"
```
4. git pull，拉取当前分支最新代码
```
git pull
```
5. push到远程master分支
```
git push origin master
```

