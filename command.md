# 命令行工具

### Mac原生命令行

`rmdir`：删除空目录。

`rm`：删除文件或目录。

`touch`：修改文件更改时间，一般用来创建文件。

`mv`：移动文件。

`pwd`：查看当前文件夹的绝对路径。

`lsof`：查看端口占用，如`lsof -i:3000`。

`cal`：查看当月日历，`cal -y 2022`查看某一年的日历。

`history`：查看命令行历史，`history | grep 需要查找的内容`。



### 开源命令行

[tree](https://github.com/owenthereal/ccat)：展开树状目录。

[ccat](https://github.com/owenthereal/ccat)：查看代码，已覆盖`cat`，直接`cat file`即可。

[jq](https://github.com/owenthereal/ccat)：读取jq文件，最常用来查看命令，`jq .scripts package.json`。

[tmux](https://github.com/tmux/tmux)：终端多任务多窗口。



### 别名清单

主要的别名设置主要在`.zshrc`中，使用`code .zshrc`打开编辑。

```shell
# git alias
git status = gs
git add .= ga
git commit = gc
git pull = gp
git push = gh
# git commit fe-notes to gitee
git add . && git commit -m 'update' && git push = gn
```

```shell
# node alias
npm --version = nv
npm run dev = nrd
npm run serve = nrs
npm run build = nrb
npm run test = nrt
npm publish = np
```

```shell
# other alias
code . = c
iconfont-manager = im
```



### 局域网穿透

```shell
# 开启本地服务
http-server ./dist -p 9090
# 内网穿透
ssh -R 80:127.0.0.1:9090 sh@sh3.neiwangyun.net
```
