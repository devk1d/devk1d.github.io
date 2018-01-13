---
layout: single
title: 两分钟搭建 Github Pages 博客
---

作为程序员，不可避免的想过搭建一个自己的博客。传统的方法需要购买域名空间，搭建 wordpress，再使用复杂的 HTML 编辑器写文章，对于“懒惰”的程序员来说，一点都不 cool

现在 Github Pages 能一键生成页面，不需要前端知识，只需要学会 Markdown 语法写文章即可，目前生成博客的库最普遍的有 Hexo 和 Jekyll，除非你要本地预览，使用哪一个没多大区别

网上已经有很多搭建的教程，但都不是最轻松的方法，要 cool 就 cool 到极致，只需两步便能开始写作

快速开始
---


### 1) Fork [jekyll-now](https://github.com/barryclark/jekyll-now) 仓库

打开 [jekyll-now](https://github.com/barryclark/jekyll-now) ，点击右上角 Fork，等待几秒钟，便创建了一个自己的镜像库

在生成的库页面，点击 Settings，把仓库名设置为[你的 Github 名字].github.io（例如我的名字是 devk1d，那就设置为 devk1d.github.io）

![](https://raw.githubusercontent.com/barryclark/jekyll-now/master/images/step1.gif)



### 2) 编辑配置文件

配置文件为 `_config.yml`，已在项目根目录生成

name 对应网站名称, description 对应描述, avatar 对应头像图片地址, github 对应自己的 github 地址，填写自己的 github 名字即可

其他配置可以根据自己需要去修改，这里不多描述了

![](https://raw.githubusercontent.com/barryclark/jekyll-now/master/images/jekyll-now-theme-screenshot.jpg)


开始写作吧
---

编辑 `/_posts/2014-3-3-Hello-World.md` 来发布自己第一篇文章吧，标题的格式就不多说了一看就明白，文件里有 layout 和 title 示例，照着写就好。



本地预览（可选）
---

如果想在本地修改文章或者一些样式，预览后再上传，那就必须安装 Ruby 环境，Mac 下自带 Ruby，Windows 和 Linux 就自行搜索安装吧。以下操作需要一定 git 知识。

1. 终端运行 `sudo gem install github-pages`，这个插件包含了 Jekyll, Sass 等库。
2. clone 你的仓库，例如 `git clone https://github.com/devk1d/devk1d.github.io.git`
3. 启动服务 `jekyll serve`，在浏览器输入 [http://127.0.0.1:4000/](http://127.0.0.1:4000/) 即可看到效果
4. 修改完成后 git push 到你的仓库即可.

其他可以 Fork 的模板
---
推荐一些不一样的模板，你可以根据以上同样的步骤 Fork 以下库，挑一个自己喜欢的吧

- [Hyde](https://github.com/poole/hyde) by MDO
- [Lanyon](https://github.com/poole/lanyon) by MDO
- [mojombo.github.io](https://github.com/mojombo/mojombo.github.io) by Tom Preston-Werner
- [Left](https://github.com/holman/left) by Zach Holman
- [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) by Michael Rose
- [Skinny Bones](https://github.com/mmistakes/skinny-bones-jekyll) by Michael Rose
