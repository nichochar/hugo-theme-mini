# Simple Theme

Simple 是一个根据 [Cactus](https://github.com/nodejh/hugo-cactus-theme) 改编的简约主题。本人在 [Cactus](https://github.com/nodejh/hugo-cactus-theme)的基础上做了一些修改，主要是添加了归档页、添加了标签页、修改了部分样式。总的来说该主题具有以下特点：

+ 自定义 “关于” 页面
+ 标签页
+ 归档页
+ Disqus 评论
+ 多说评论
+ RSS 订阅
+ 语法高亮

![Screenshot](https://raw.githubusercontent.com/digitalcraftsman/hugo-cactus-theme/dev/images/screenshot.png)


## 安装

进入 `hugo` 的站点目录运行下面的命令：

```
$ cd themes
$ git clone https://github.com/nodejh/hugo-theme-simple.git
```


## 示例站点

[`exampleSite`](https://github.com/nodejh/hugo-theme-simple/tree/master/exampleSite) 是本主题的一个示例站点，里面有配置文件、关于页面的一些示例。


### 配置文件

本主题提供了一个示例配置文件是 [`exampleSite`](https://github.com/nodejh/hugo-theme-simple/tree/master/exampleSite) 目录里的 [`config.toml`](https://github.com/nodejh/hugo-theme-simple/blob/master/exampleSite/config.toml) 文件。

配置文件中对大部分配置都有详细的注释说明，复制该文件到站点目录下，根据自己的情况修改即可。


## 头像

你可以将 [images](https://github.com/nodejh/hugo-theme-simple/blob/master/static/images/) 目录下的 `avatar.png`、`avatar@2x.png`  和 `favicon.ico` 都替换为你自己的图像。


## 关于页面

使用关于页面首先要在你的站点目录的 `content` 目录下创建一个 `about` 目录，然后再创建一个 `index.md` 文件，编写该文件即可。

你也可以参考本主题示例站点中的关于页：[`exampleSite/content/about/index.md`](https://github.com/nodejh/hugo-theme-simple/blob/master/exampleSite/content/about/index.md)。


## 隐藏页面

如果你不想让一个页面出现在文章列表中，只需要在 markdown 文件的 `frontmatter` 中添加 `hidden = true` 即可。

然后你可以在其他任何地方通过链接来引用该页面，如在菜单中放置一个链接。

关于页面就是这么实现的。


## Disqus 评论

本主题提供两种评论系统，Disqus 和多说。使用 Disqus 评论需要在 `config.toml` 进行设置。

设置 `disqusShortname` 为你的 Disqus ID，并将 `enableDisqus` 设置为 `true` 即可开启 Disqus 评论。

将 `enableDisqus` 设置为 `false` 则不启用 Disqus 评论。


## 多说评论

由于在中国大陆无法使用 Disqus，所以本主题提供了多说评论系统。多说评论系统的配置和 Disqus 配置基本一致。


## 不使用评论系统

由于使用第三发评论系统会使网站加载速度变慢，所以也可以不使用评论系统。只需要将 `enableDisqus` 和 `enableDuoshuo` 都设置为 `false` 即可。

然后我的博客由于同步到了 Github Issues，所以也同时在主题中提供了跳转到 Github Issues 评论的文字提示。只需要设置 `enableGithubIssuesTips = true` 即可。当然，一般是不需要这么做的，这可能只是我个人需求。具体效果可以参考我的博客 [http://nodejh.com](http://nodejh.com)。


## 社交链接

本主题的社交链接是字体图标的样式，并放置在了页面底部。你可以通过在 `config.toml` 的 `social` 模块中修改添加你的社交链接。社交链接提供了两种字体图标，选用其中一种即可：

- [Font awesome](https://fortawesome.github.io/Font-Awesome/) 或
- [Mono social icons](https://github.com/drinchev/monosocialiconsfont)

`iconFont` 变量即字体图标库，可以是 `font-awesome` 或 `mono-social`。

如果使用的是 `Mono social icons` 即 `iconFont = "mono-social"`，则图标还有三种可选样式：`-circle`、`rounded`、或默认 `empty`。


## 部署主题

配置完成之后，就可以使用下面的命令来启动 hugo 服务编译 markdown 文件生成静态站点：

```
$ hugo server
```

然后在浏览器地址栏输入 [`localhost:1313`](http://localhost:1313) 来访问站点。


## License

[MIT](https://github.com/nodejh/hugo-theme-simple/blob/master/LICENSE.md)

## 鸣谢

特别感谢 [digitalcraftsman](https://github.com/digitalcraftsman) 的 [Cacuts](https://github.com/digitalcraftsman/hugo-cactus-theme) 主题：

- [hugo-cactus-theme](https://github.com/digitalcraftsman/hugo-cactus-theme)
