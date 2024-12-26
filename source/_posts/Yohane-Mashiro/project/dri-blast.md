---
title: 目录爆破工具
date: 2024-12-26 20:04:00
cover: https://avatars.githubusercontent.com/u/78677516?v=4
tags:
  - ctf工具
categories:
  - Yohane-Mashiro
---

# dir-blast （目录爆破）

闲的发慌，顺手做了这个小工具
项目地址：[Ciallo～(∠・ω＜)⌒☆](https://github.com/Yohane-Mashiro/dir-blast)
一个用于 CTF 的快速目录扫描工具
希望有用吧
```
--------------------------------------------------------------
|      _   _                  _       _                 _    |
|   __| | (_)  _ __          | |__   | |   __ _   ___  | |   |
|  / _` | | | | '__|  _____  | '_ \  | |  / _` | / __| | __| |
| | (_| | | | | |    |_____| | |_) | | | | (_| | \__ \ | |_  |
|  \__,_| |_| |_|            |_.__/  |_|  \__,_| |___/  \__| |
--------------------------------------------------------------
```

## 功能

- 使用字典文件对目标 URL 进行目录暴力破解
- 支持多线程，提高扫描速度

## 使用方法

### 从源码运行

1. 克隆仓库到本地：
    ```sh
    git clone https://github.com/Yohane-Mashiro/dir-blast.git
    ```
2. 进入项目目录：
    ```sh
    cd dir-blast
    ```
3. 安装依赖：
    ```sh
    pip install -r requirements.txt
    ```
4. 运行脚本：
    ```sh
    python main.py -u <目标URL>
    ```

### 使用 Release

你也可以从 [Release 页面](https://github.com/Yohane-Mashiro/dir-blast/releases) 下载最新的可执行文件。

## 参数说明

- `-u` 或 `--url`：目标 URL 地址（必填）
- `-w` 或 `--wordlist`：字典文件路径（默认: `dictionary.txt`）
- `-t` 或 `--threads`：线程数（默认: 50）

-----