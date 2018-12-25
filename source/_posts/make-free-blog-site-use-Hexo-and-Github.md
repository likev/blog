---
title: 使用 Hexo 写作以及在 GitHub 建立个人博客
date: 2016-03-27 17:50:48
updated: 2018-12-25 14:00:00
---

GitHub Pages 提供了免费的空间让大家可以做静态站点，还能够绑定自己的域名，这么好的东西一定要试一下了。

Hexo 是一个基于 Node.js 的静态博客生成程序，你用 Markdown 语法写一些文章，然后它帮你转化为一个博客网站。安装 Hexo 前需先安装 Node.js 和 Git 。
具体的安装说明见官方文档。下面是发布文章的方法。

### 一. 新建文章

``` bash
$ hexo new "My New Post"
```
或者手动在 `source/_posts` 目录下新建一个 Markdown 文件或 html 文件开始写新文章。

<!-- more -->

Front-matter 是文件最上方以 --- 分隔的区域，用于指定个别文件的变量，举例来说：
```yaml
title: Hello World
date: 2013/7/13 20:46:25
---
```
以下是预先定义的参数，您可在模板中使用这些参数值并加以利用。

| 参数 | 描述 | 默认值 |
|---|---|---|
| layout | 布局 | post |
| title |	标题 	 | '' |
| date |	建立日期  |	文件建立日期 |
| updated |	更新日期  |	文件更新日期 |
| comments |	开启文章的评论功能  | true |
| tags |	标签（不适用于分页） 	 | |
| categories |	分类（不适用于分页）  |	|
| permalink | 覆盖文章网址 	 | |

写文章时可以插入 `<!-- more -->` 来提示在主页的文章列表显示`...阅读全文`链接。

### 二. 运行本地服务器 实时预览新文章

``` bash
$ hexo server
```
当然你可以不预览直接进行下述步骤

### 三. 生成静态文件

``` bash
$ hexo generate
```
或简写为
``` bash
$ hexo g
```
上述命令会将 source 目录的 markdown 文件和 html 文件根据 layout 进行解析（比如按相应语法处理后插入到主页和文章页的某个 div 内）然后和 source 目录的其他文件（如图片、JavaScript、CSS、音乐等文件）一并放于 public 目录下。public 目录即是你的静态网站目录。

如果不想被解析，可将 layout 设为 false，此时在主页仍能看到此文章链接，但打开文章进入文章页时为原始 html 文件（即不插入文章页某个 div 内）

如果不需要部署至远程服务器，可省略下述步骤。

### 四. 部署至 GitHub 并绑定域名

``` bash
$ hexo deploy
```
上述命令会将 public 目录上传至 GitHub 服务器。实际是 Hexo 将 public 目录复制到 .deploy_git 目录，然后调用 `git push` 命令将 .deploy_git 目录下的文件提交至 `gh-pages` 分支中。

步骤三和四可合并为 `$ hexo deploy -g` 写好文章后只需用这一条命令即可发布至网站

#### GitHub Pages 绑定域名方法

1. 新建项目  `https://github.com/username/projectname` ，并将 `gh-pages` 设为默认分支
2. 在上述 `gh-pages` 分支中添加一个文件，文件名为 `CNAME`，内容为你的域名 `blog.sample.com`
3. 在域名服务商处将 `blog.sample.com` CNAME 至 `username.github.io`
4. 域名解析可能需要一定时间，等待即可

> 1. Hexo官方网站文档：[documentation](https://hexo.io/docs/)
> 2. GitHub Pages域名设置官方文档：  [using-a-custom-domain-with-github-pages](https://help.github.com/articles/using-a-custom-domain-with-github-pages/)
