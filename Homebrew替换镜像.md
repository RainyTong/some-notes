## 替换及重置Homebrew默认源
> 转自[替换及重置Homebrew默认源](https://lug.ustc.edu.cn/wiki/mirrors/help/brew.git)

替换brew.git:
```
cd "$(brew --repo)"
git remote set-url origin https://mirrors.ustc.edu.cn/brew.git
```

替换homebrew-core.git:
```
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://mirrors.ustc.edu.cn/homebrew-core.git
```

---
在中科大源失效或宕机时可以： 

1. [使用清华源设置参考](https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/)


2. 切换回官方源：

重置brew.git:
```
cd "$(brew --repo)"
git remote set-url origin https://github.com/Homebrew/brew.git
```

重置homebrew-core.git:
```
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://github.com/Homebrew/homebrew-core.git
```
