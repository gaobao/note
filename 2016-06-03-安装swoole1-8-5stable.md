---
title: 安装swoole1.8.5stable
date: 2016-06-03 16:03:40
tags: [php,swoole]
---

>安装php扩张swoole,[官网](http://wiki.swoole.com/wiki/page/6.html)给出详细方法,我还是记一下自己的
+ <!-- more -->
<The rest of contents | 余下全文>
```shell
#linux环境 ubuntu16.04
#php 5.6.22
#下载[swoole stable](https://github.com/swoole/swoole-src/releases/tag/swoole-1.8.5-stable)
cd swoole-src-swoole-1.8.5-stable
phpize
./configure
make
sudo make install
#最后在php.ini加extension=swoole.so
sudo vim /etc/php/5.6/cli/php.ini
#最后使用php-m 查看swoole 是否以正确安装
```