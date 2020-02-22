---
layout: page
title: 常见问题
links:
  repo: https://github.com/xaoxuu/hexo-theme-volantis
  bug: https://github.com/xaoxuu/hexo-theme-volantis/issues/new?assignees=&labels=BUG&template=bug-report.md
  doubt: https://github.com/xaoxuu/hexo-theme-volantis/issues/new?labels=疑问&template=question-report.md
  idea: https://github.com/xaoxuu/hexo-theme-volantis/issues/new?assignees=&labels=建议&template=feature-request.md
---

::: success
通常来说，一个全新的工程全部使用默认配置是正常没有故障的。
:::

[<i class='fas fa-play-circle'></i> 示例博客1](https://xaoxuu.com) &nbsp;&nbsp;&nbsp; [<i class='fas fa-play-circle'></i> 示例博客2](https://mxclub.github.io)

如果无法使用或者效果与示例有较大区别，可以使用hexo官方提供的用于单元测试的博客应用本主题查看样式是否正常，对比 `_config.yml` 文件排查问题。

> Hexo官方的单元测试项目： [https://github.com/hexojs/hexo-theme-unit-test.git](https://github.com/hexojs/hexo-theme-unit-test.git)


## 如何更新主题

使用主题的时候，尽量fork主题到自己的GitHub，然后进行修改并使用。这样做的好处是：当主题进行重要更新的时候可以根据需要拉取合并代码，使自己DIY的主题能够通过更新获取BUG修复或者新特性。

如果不懂请自行搜索关键词：fork 更新

## 无法成功运行本地预览

可能是没有安装依赖，请按照【开始使用 -> 下载安装】中的步骤进行安装，并安装所需依赖。

如果开启了某些第三方服务，请查看文档中是否要求安装插件。

如果报错信息有 `lastIndex`，你可以尝试把博客根目录配置文件中找到 `highlight`，并将 `auto_detect` 设置为 `false`。


## 主题配置修改没有生效

请确认文档中要求修改的是博客主目录的配置文件 `./config.yml` 还是主题的配置文件 `themes/volantis/config.yml`。

## 主题样式修改没有生效

如果主题配置文件中开启了cdn服务，那么修改本地的样式是不会生效的，需要关闭cdn服务。

## 修改什么都没有生效

需要 `hexo clean` 然后重新 `hexo s`

如果安装了「相关文章推荐」插件后，每次修改front-matter后都需要重新 `hexo s`

## 搜索无法使用

1. 检查是否安装文档要求正确的安装了依赖包。
2. 检查根目录配置文件是否有search字段冲突。
3. 如果以上两步都无法找到问题，请下载示例源码进行对比。

## 搜索结果链接不正确

请检查根目录配置文件中的链接是否正确，如：

```yaml 站点配置文件
url: https://xaoxuu.com
root: /
```

## 关于SEO

SEO跟主题之间没有什么耦合，所以主题没有捆绑SEO插件，你需要的话可以自己安装，我安装了以下SEO优化插件：

- [hexo-autonofollow](https://github.com/liuzc/hexo-autonofollow)
- [hexo-generator-seo-friendly-sitemap](https://github.com/ludoviclefevre/hexo-generator-seo-friendly-sitemap)

## 教程与指南

亲这里是MaterialX主题的使用文档，不是Hexo博客一站式教程。与MaterialX主题无关的，例如markdown的写法、Valine的用法以及BUG之类的，请自行搜索相关教程。

请一定要阅读官方文档！ [Hexo官方文档](https://hexo.io) | [Valine官方文档](https://valine.js.org)

<img src="https://cdn.jsdelivr.net/gh/xaoxuu/volantis@1.0/img/aru/161.png" style="width:100%">
