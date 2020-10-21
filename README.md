# 我的 dmenu 构建

dmenu 是一个极简应用程序选择器

## 要求

构建 dmenu 前, 你需要有 Xlib 头文件

## 安装

编辑 config.mk 来匹配你的本地设置 (dmenu 将默认安装在 /usr/local)
之后通过以下命令安装 dmenu (必须使用 root 用户):

```shell
make clean install
```

## 自定义补丁

### 打补丁

```shell
patch < [patch file]
```

#### patches

1. fuzzymatch

> [fuzzymatch](https://tools.suckless.org/dmenu/patches/fuzzymatch/) 默认启动搜索模糊匹配，加 `-F` 禁用搜索模糊匹配，加 `-i` 不区分大小写

2. fuzzyhighlight

> [fuzzyhighlight](https://tools.suckless.org/dmenu/patches/fuzzyhighlight/) 高亮显示模糊匹配

3. center

> [center](https://tools.suckless.org/dmenu/patches/center/) 加 `-c` dmenu 居中在屏幕中间

4. grid

> [grid](https://tools.suckless.org/dmenu/patches/grid/) 加`-g` 设置搜索显示列数和加 `-l` 设置搜索显示行数

5. numbers

> [numbers](https://tools.suckless.org/dmenu/patches/numbers/) 右上角显示匹配项和总数的文本

## 运行 dmenu

```shell
dmenu_run
```
