# github commit process
> *if origin exists:*

```
git remote rm origin
```
Then:
1. 初始化本地仓库

```
git init
```

2. add要上传的文件

```
git add <>
```
如果要将当前文件夹下的全部文件上传，可以
`git add .`

3. 提交并注释
```
git commit -m "comments..."
```

4. 连接远程仓库并起别名为: origin
```
git remote add origin git@github.com:rainytong/test.git
```
5. **pull**一下
```
git pull --rebase git@github.com:rainytong/test.git

```

6. **push**一下
```
git push -u origin master
```

搞定啦嘻嘻（just 给自己备忘一下:wink:）
