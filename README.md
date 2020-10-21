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

## 运行 dmenu

```shell
dmenu_run
```
