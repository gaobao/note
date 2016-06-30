---
title: ubuntu下安装php，mysql，apache
date: 2016-06-03 16:03:07
tags:
---

### 安装apache
```shell        
    sudo apt-get update
    sudo apt-get install apache2
```
+ <!-- more -->
<The rest of contents | 余下全文>

### 安装mysql
```shell
    sudo apt-get install mysql-server
```
安装过程中还需输入mysql密码
### 安装php
```shell
#sudo apt-get install php5 //由于我的ubuntu 版本是16.04,所以改语句会报错
sudo add-apt-repository ppa:ondrej/php5
sudo add-apt-repository ppa:ondrej/php5-5.6
#添加php的库
sudo apt-get update
sudo apt-get install php5.6
```


