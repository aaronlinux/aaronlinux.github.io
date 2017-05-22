---
layout: post
title: Linux/Mac terminal学习笔记
tags:
- 练习
- Linux
categories: 学习
---
关于 command line 的学习笔记




* content
{:toc}
## 文件系统的定位导航

显示当前路径

> pwd

切换目录

> cd

列出当前目录下的文件

> ls

显示隐藏文件

> ls -a


## 操作文件／创建／改名等

创建文件夹

> mkdir 文件夹的名字

创建新的文件

> touch 文件名称

拷贝文件

> cp 文件名称 新的文件路径

重名文件

> mv 旧文件名称 新的文件名称

删除文件

> rm

## 查找命令

查找文件

> find

查找当前目录的所有文件

> find .

查找特定路径下的所有的文件

> find 需要查看的路径

只看路径不看下面的文件

> find . -type d

只看文件不看路径

> find . -type f

在当前路径下需要某个文件，文件名中可以只用通配符。这里面把name换乘iname，就可以忽略文件的大小写。

> find .type f -name “文件名”

在当前路径下寻找特定修改时间的的文件

> find . -type f -mmin -10
在十分钟之内，修改过的文件

> find . -type f -mmin +10
在十分钟之前，修改过的文件

> find . -type f -mmin +1 -mmin -5
在五分钟以内，一分钟之前的时间内修改过的文件

有些时候后，我们不用分钟，可能用的天数 -mmin改成 -mtime

这里面m表示modify，意味着modify的时间；

有的时候我们会用access的时间，也就是说 -amin或者 -atime

还有的时候会用到change的时间，也就是说 -cmin或者 -ctime