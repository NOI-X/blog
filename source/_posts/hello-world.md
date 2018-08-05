---
title: Toturial of NOI-X.github.io
---

## Quick Start

首先在你的电脑上安装基础环境：Nodejs、yarn、git

### Install Nodejs on Windows

1. [下载](https://nodejs.org/dist/v8.11.3/node-v8.11.3-x64.msi)
2. 打开并安装

### Install Nodejs on Ubuntu

```
# install nodejs on ubuntu -version 8.x

curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt install -y nodejs

```

### Install git on windows

1. [下载](https://github.com/git-for-windows/git/releases/download/v2.18.0.windows.1/Git-2.18.0-32-bit.exe)
2. 打开并安装

### Install git on Ubuntu

```
sudo apt install git
```

### Install yarn

跟随yarn的[文档](https://yarn.bootcss.com/docs/install/)页面指引即可。

## Init the project at the first time

1. 你要有一个Github账号，右转[Github](https://github.com)自行注册。
2. 联系QQ:1075324834@qq.com 将你添加到Github的组织内。
3. 学会初步使用Git和Node，包括如何Clone项目，如何用yarn安装Node的依赖。

### Clone the blog project from github

```
git clone git@github.com:NOI-X/blog.git
```

### Install the package of this project

进入你clone下来的目录，然后使用yarn直接安装所有依赖环境。

```
# On Ubuntu

cd ./blog
yarn install
```

**检查是否安装成功**
```
hexo s
```
打开：http://localhost:4000， 如何可以看到页面即成功。

## Add your article to NOI-X.github.io

命令行中：
``` bash
hexo new myarticle
```
或直接在`./blog/source/_posts/`文件夹下新建一个名为`myarticle.md`的文件。但这种做法会丢失如本文件前几行的内容。

编写这个文件即可。

### Check your article at localhost

```
hexo clean
hexo g
hexo s
```

### Upload articles to NOI-X.github.io

```
hexo clean
hexo g
hexo d
```

### Push this project to github

``` bash
git add ./source
git commit -m 'say somthing'
git push origin master
```


### HEXO MARKDOWN Syntax

| 基本操作 | 方法|
|:---------|:----|
|添加链接  | `[文字](链接)` |
| 添加图片 | 先把图片文件复制到`./source/img/`中，然后在md中：`[](/img/pic.png)`|
| 其他操作 | 参考别人的代码或Google |
