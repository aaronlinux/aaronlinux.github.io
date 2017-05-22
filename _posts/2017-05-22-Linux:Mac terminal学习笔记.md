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
## 文件的定位导航

显示当前路径

> pwd

切换目录

> cd

列出当前目录下的文件

> ls

显示隐藏文件

> ls -a


## 操作文件

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

> find .type f -name “文件名” -maxdepth 1

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

假设我们想找到目录内的文件大小超过5M的东西，我们就可以使用这样的命令

> find . -size +5m
我们可以发现，命令行里➕一般表示大于，➖就表示小于。
这里面我们用的M表示兆，小写k表示千字节，大写的G表示Gib字节

找到当前目录下的空文件

> find . -empty

根据文件权限来寻找文件

> find . -perm 777

注：输出结果继续执行其他的命令，我们可以接一个这样的参数
> -exec rm {} +
这里面的rm是可以换成其他它的命令的。表示前面输出的结果嵌入后面的命令,这里的加号表示命令结束的符号。

## curl的使用

curl是可以直接接上网络地址的。可以返回跟对应网址有关的信心，具体使用方法就比较复杂了。

## 个性化制定bash

> touch .bash_profile
> 
> touch .bashrc

.bash_profile 是一定会被体现在bash的，为了让bashrc的修改也体现在bash里面，我们需要在bash_profile里面加入语句：

> if [ -f ~/.bashrc ]; then

> source ~/.bashrc

> fi

## 修改bash的颜色

一般来说直接修改.bashrc

> PS1=“-> ”;
> 
> export PS1;
这里面的可以添加系统可识别的字段

> \h the hostname to the first 主机名

> \n newline 新一行

> \s the name of the shell 命令解释器的名称

> \t the current time in 24-hour format 时间24小时的格式

> \u the username of the current user 当先用户的名称

> \w the current working directory 当前工作路径

> \W the base name of the current working directory 当前工作路径位置的名称

更改颜色和可以用tput命令，举例子：
> PS1=“$(tput setaf 166)\u@$(tput setaf 228)\h-> ”;
> 
> PS1+=“$(tput setaf 71)\W”;
> 
> PS1+=“$(tput sgr0)”;
> 
> export PS1; 

