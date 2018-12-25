---
title:  使用 Caddy 给网站添加 HTTPS 和 HTTP2 支持
date:  2017-03-05 11:05:00
tags:
- HTTPS
- HTTP/2
---

## Caddy 介绍
Caddy 是一个快速的、开源的、跨平台的（Windows, Mac, Linux, BSD, and Android） HTTP/2 网站服务器，它自动支持 HTTPS 访问。官方网站为 https://caddyserver.com/ ，项目 GitHub 地址为 https://github.com/mholt/caddy 。

## Caddy 特色

1. 配置简单
2. 自动获取、管理和更新 Let's Encrypt 的免费 SSL/TLS 证书
3. 默认启用更快的 HTTP/2 协议
4. 支持单一服务器部署多个站点（虚拟主机），通过 TLS SNI 为所有站点添加 HTTPS 支持
5. Caddy 默认是静态文件服务器，但它支持 FastCGI，所以支持 PHP 等
6. 支持扩展，你可以编程添加更多功能
7. 跨平台，无需额外程序或环境依赖
8. 支持反向代理（Reverse Proxy）和负载均衡。所以你可以保持现有的网站架构不变，仅把 Caddy 用做前端代理。

![](/images/caddy-features.png)
<!-- more -->
## Caddy 安装
可以通过 https://caddyserver.com/download 页面勾选需要的额外功能，按需下载不同平台的安装文件；也可以通过命令 `curl https://getcaddy.com | bash` 一键自动部署。

## Caddy 配置
Caddy 默认使用当前所在目录名为 Caddyfile 的配置文件，在 Caddyfile 文件中输入 `localhost:8080` 然后运行 `caddy` 命令即可启动一个静态文件网站服务器，服务器根目录默认为当前目录。

你也可以像下面这样配置多个网站，并指定压缩或日志等。
```apache
mysite.com {
    root /www/mysite.com
}

sub.mysite.com {
    root /www/sub.mysite.com
    gzip
    log ../access.log
}
```
像上面这样使用域名时，Caddy 默认会从 Let's Encrypt 获取免费的 SSL/TLS 证书。证书密钥默认存放在用户主目录（`$HOME` 环境变量）下的 `.caddy` 文件夹中，Caddy 会自动管理并更新密钥。

Caddy 文档( https://caddyserver.com/docs )有其他配置的详细说明，如前向代理、负载均衡、URL 重写、XMLHttpRequest2 和 WebSocket 支持等。

## Caddy 部署
Linux 下普通用户无法绑定小于 1024 的端口，但又不想让 Caddy 以 root 用户身份运行，可以用类似如下命令解决这个问题：
```bash
sudo setcap cap_net_bind_service=+ep ./caddy
```
Caddy 并没有提供类似 apache 的系统服务功能，但你可以用 `nohup caddy &` 这样的命令让 Caddy 在后台运行。也有一些社区贡献的启动脚本可供使用：https://github.com/mholt/caddy/tree/master/dist/init 。
