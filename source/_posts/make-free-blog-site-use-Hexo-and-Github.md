---
title: 使用 Hexo 在 GitHub 建立个人博客
date: 2016-03-27 17:50:48
---

GitHub Pages 提供了免费的空间让大家可以做静态站点，还能够绑定自己的域名，这么好的东西一定要试一下了。

Hexo 是一个基于 Node.js 的静态博客生成程序，你用 Markdown 语法写一些文章，然后它帮你转化为一个博客网站。安装 Hexo 前需先安装 Node.js 和 Git 。
具体的安装说明见官方文档。下面是发布文章的方法。

### 一. 新建文章

``` bash
$ hexo new "My New Post"
```
或者手动在 `source/_posts` 目录下新建一个 Markdown 文件开始写新文章。

<!-- more -->

### 二. 运行本地服务器 实时预览新文章

``` bash
$ hexo server
```
当然你可以不预览直接进行下述步骤

### 三. 生成静态文件

``` bash
$ hexo generate
```
上述命令会将 source 目录的 markdown 文件转化为 html 文件然后和 source 目录的其他文件（如图片音乐文件）一并放于 public 目录下。

public 目录即是你的网站目录，你也可将 html 或 图片文件直接放在此目录。

### 四. 部署至远程站点

``` bash
$ hexo deploy
```
上述命令会将 public 目录上传至 GitHub 服务器。实际是 Hexo 将 public 目录复制到 .deploy_git 目录，然后调用 `git push` 命令将 .deploy_git 目录下的文件提交至 `gh-pages` 分支中。

步骤三和四可合并为 `$ hexo deploy -g` 写好文章后只需用这一条命令即可发布至网站

### GitHub Pages 绑定域名方法

1. 新建项目  `https://github.com/username/projectname` ，并将 `gh-pages` 设为默认分支
2. 在上述 `gh-pages` 分支中添加一个文件，文件名为 `CNAME`，内容为你的域名 `blog.sample.com`
3. 在域名服务商处将 `blog.sample.com` CNAME 至 `username.github.io`
4. 域名解析可能需要一定时间，等待即可

> 1. Hexo官方网站文档：[documentation](https://hexo.io/docs/)
> 2. GitHub Pages域名设置官方文档：  [using-a-custom-domain-with-github-pages](https://help.github.com/articles/using-a-custom-domain-with-github-pages/)
