---
layout: post
title: "2019.7.21 学习日志"
date: 2019-07-21
tag: 日志
---

### 今日学习内容

1. 完善博客

2. 学习 Linux 操作

3. 远程管理命令 ssh

   ```
   ssh [-p prot] user@remote
   ```

   `user`: 远程机器上的用户名

   `remote`:远程机器的地址

   `port`:SSH Server 监听的端口号
   
4. 远程传输文件/目录

   ```
   # 把当前目录下的1.txt 文件 复制到远程家目录下的 Desktop/1.txt
   scp -P port 1.txt user@remote：Desktop/1.txt
   
   # 把远程家目录下的 Desktop/1.txt 复制到当前目录下的 1.txt
   scp -P port user@remote:Desktop/1.txt 1.txt
   
   # 加上 -r 可以传输文集案件
   # 把当前目录下的 demo 文件夹复制到远程家目录下的 Desktop
   scp -r demo user@remote:Desktop
   
   # 把远程家目录下的Desktop 复制到当前目录下的 demo 文件夹
   scp -r user@remote:Desktop demo
   
   ```

   
