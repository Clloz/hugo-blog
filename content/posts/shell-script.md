---
title: "Shell Script"
date: 2023-05-20T10:43:51+08:00
draft: true
---

### 前言

记录一些遇到的 shell 脚本知识点

### 知识点

#### 判断文件是否存在

```bash
if [-f filename]; then
	echo "file exsit"
else
	echo "file does not exist"
fi
```

#### 引号

引号中只有元字符有特殊意义，如果使用 `~` 作为 home 目录，则不要放到引号中，否则路径无法正确解析，参考[Tilde (~/) not working on if then statement in Shell script](https://stackoverflow.com/questions/27238491/tilde-not-working-on-if-then-statement-in-shell-script)

 
