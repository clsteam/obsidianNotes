---
{"dg-publish":true,"permalink":"/100-inbox/study/github/","tags":["学习","gardenEntry"]}
---


## Metadata
Status::    #笔记状态/🌱发芽
Source Type::  #📥/📰️文章
Author:: yao
Source URL:: 

# Github 加速
### Windows 系统：
1. 下载替换 host 文件 https://raw.hellogithub.com/hosts
2. 将下载的文件内容添加到 `C:\Windows\System32\drivers\etc` 文件夹里面的 host，如果原文件夹没有 host 文件，直接复制进去即可
3. `win+R` 输入 `cmd`，敲入 `ipconfig /flushdns` 回车，清除 DNS 缓存
4. 大功告成

### Mac 系统
1. 下载替换 host 文件 https://raw.hellogithub.com/hosts
2. 打开终端（`command+space`，输入 `terminal` 回车），输入 `sudo vi /etc/hosts`，回车，会要求输入密码，输入密码即可。
3. 将下载的文件内容添加到上述文件末尾，如果原文件没有内容，直接复制进去即可，`Esc` `:wq` 保存并退出
4. 刷新 DNS 缓存，
	1. OS X 12 (Sierra) and later 系统：
	2. `sudo killall -HUP mDNSResponder`
	3. `sudo killall mDNSResponderHelper`
	4. `sudo dscacheutil -flushcache` 
	5. OS X 11 (El Capitan) and OS X 12 (Sierra) 系统：
	6. sudo killall -HUP mDNSResponder
6. 大功告成

