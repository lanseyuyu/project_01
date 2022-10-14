# git 配置

## 1.用户名和邮箱配置

```git
1. git config --global user.name "xxx"
2. git config --global user.email "xxxxx"
```

C盘 user ----> gitconfig （设置成功）

<img src="file:///C:/Users/zxm_pc/AppData/Roaming/marktext/images/2022-10-13-11-02-09-image.png" title="" alt="" width="490">

查询全局配置型

```git
 git config --list --global
 git config user.name
 git config user.email
```

帮助命令

git help config

git config -h 

## 2. git的基本操作

#### 1.git本地仓库目录初始化

@1 目录右键打开‘git bash’

@2 git init命令初始化

### 2.git工作区的几个工作状态

![](C:\Users\zxm_pc\AppData\Roaming\marktext\images\2022-10-13-22-06-33-image.png)

1. 检查文件的状态

![](C:\Users\zxm_pc\AppData\Roaming\marktext\images\2022-10-13-22-28-58-image.png)

untracked file 未跟踪的文件（git未管理）

2. 精简方式显示文件的状态

```git
git status -s
git status --short
```

![](C:\Users\zxm_pc\AppData\Roaming\marktext\images\2022-10-13-22-33-15-image.png)

3. 跟踪新文件

```git
git add git.md
```

![](C:\Users\zxm_pc\AppData\Roaming\marktext\images\2022-10-13-22-36-34-image.png)

4. 提交更新

```git
git commit -m "提交的消息"
```

![](C:\Users\zxm_pc\AppData\Roaming\marktext\images\2022-10-13-22-40-14-image.png)

5. 对已提交文件进行修改（检查状态）

![](C:\Users\zxm_pc\AppData\Roaming\marktext\images\2022-10-13-22-45-10-image.png)

6. 修改的文件提交暂存区

![](C:\Users\zxm_pc\AppData\Roaming\marktext\images\2022-10-13-22-47-54-image.png)

7. 修改的文件提交仓库

![](C:\Users\zxm_pc\AppData\Roaming\marktext\images\2022-10-13-22-51-59-image.png)

8. 撤销对文件的修改（从仓库还原、覆盖文件）

```git
git checkout --xx(文件名)
```

![](C:\Users\zxm_pc\AppData\Roaming\marktext\images\2022-10-14-08-07-04-image.png)

9. 一次性提交修改和未跟踪文件

```git
git add .
```

10. 取消暂存区的文件

```git
git reset Head
git reset Head .(一次性取消)
```

![](C:\Users\zxm_pc\AppData\Roaming\marktext\images\2022-10-14-08-32-24-image.png)

11. 跳过暂存区直接提交到仓库区

```git
git commit -a -m "xxxx"
```
