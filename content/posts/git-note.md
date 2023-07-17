---
title: "Git Note"
date: 2023-05-24T21:21:25+08:00
draft: true
---

### 前言

平时使用 git 遇到的一些问题和解决方案

### git hooks 不执行

如果使用了 husky，可能是 husky 修改了 git 的默认 hooks 文件夹路径导致的，可以使用如下命令查询和调整

```bash
git config --get core.hooksPath
git config --unset core.hooksPath # 恢复默认路径
```

### git pager 设置

git 默认 branch diff show 等命令式用 pager 打开，默认 pager 是 less，可以修改指定命令的 pager

```shell
git config --global core.pager less
git config --global pager.branch ''
```

### git 删除 submodule

[git remove submodule](https://stackoverflow.com/questions/20929336/git-submodule-add-a-git-directory-is-found-locally-issue)

