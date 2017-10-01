--- 
layout:     post 
title:      Windows10下JAVA环境变量的设置 
subtitle:   Windows10配置与windows7配置有些区别  
date:       2017-10-01 
uthor:      Z.y 
header-img: img/post-bg-2015.jpg
catalog:  true
tags: 
    - JAVA
---



>windows10下主要配置三个环境变量：CLASSPATH,JAVA_HOME,Path，下面分别介绍这三个环境变量：

# CLASSPATH环境变量
CLASSPATH环境变量，变量值应该设置为

    .;%JAVA_HOME%\lib;%JAVA_HOME%\lib\tools.jar
     
注意前面的".;"一句点一分号

# JAVA_HOME环境变量
JAVA_HOME环境变量，变量值应该设置为你安装的JDK的路径，在这路径下你应该能够找到bin、lib等目录。
如果你使用的是默认安装目录，则设置如下：

    C:\Program Files\Java\jdk-9

我这里安装的是JDK-9，具体的安装路径和版本根据你自己的配置来。

# Path环境变量
Path环境变量，变量值尤其要注意，windows10版本与之前版本的配置有些不同。此处的变量值需要设置成
JDK的绝对路径。如果采取的默认安装目录，则设置如下：

    C:\Program Files\Java\jdk-9\bin;C:\Program Files\Java\jdk-9\jre\bin;
    
需要注意两个冒号的位置，不能丢


