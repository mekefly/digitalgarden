---
{"dg-publish":true,"permalink":"/100/yum/"}
---

#软件
#100-项目 

[[100-项目/linux软件安装\|linux软件安装]] [[100-项目/常用工具软件\|常用工具软件]]

一：Yum 简介
Yum（全称为 Yellow dog Updater, Modified）是一个在Fedora和RedHat以及CentOS中的Shell前端软件包管理器。基于RPM包管理，能够从指定的服务器自动下载RPM包并且安装，可以自动处理依赖性关系，并且一次安装所有依赖的软件包，无须繁琐地一次次下载、安装。


参考：
[CentOS 中用 Yum 安装、卸载软件_sunylat的专栏-CSDN博客_yum卸载](https://blog.csdn.net/sunylat/article/details/81869513)


## 二：常用的 Yum 命令

### 1、显示已经安装的软件包
>yum list installed

### 2、查找可安装的安装包
>yum list tomcat

### 3、安装软件包 （以 tomcat 为例
>yum install tomcat

### 4、卸载
>yum remove tomcat

### 5、列出软件包的依赖 （以 tomcat 为例）
yum deplist tomcat

### 6、-y 自动应答yes

我们可以用 -y 来应答所有的 yes , 比如我们安装 tomcat 的时候，用下面的命令，将安装任务一气呵成，不会中断。
例如
>yum -y install tomcat


### 7、info 显示软件包的描述信息和概要信息

>yum info tomcat

### 8、升级软件包

yum update

升级某一个软件包 ，以升级 tomcat 为例、
>yum update tomcat

检查可更新的程序
>yum check-update

 ## Yum 可视化图形界面 Yumex
 
### 1、yumex 安装
>yum install yumex