---
layout: page
group: docs
title: Site Settings「站点配置」
cover: false
meta:
  header: [title, author, updated]
btns:
  repo: https://github.com/xaoxuu/hexo-theme-volantis
  bug: https://github.com/xaoxuu/hexo-theme-volantis/issues/new?assignees=&labels=BUG&template=bug-report.md
  doubt: https://github.com/xaoxuu/hexo-theme-volantis/issues/new?labels=疑问&template=question-report.md
  idea: https://github.com/xaoxuu/hexo-theme-volantis/issues/new?assignees=&labels=建议&template=feature-request.md
---

如无特殊说明，本页面的配置信息写在 <red>**博客根目录**</red> 的 `_config.yml` 文件中。


## 多语言支持

```yaml blog/_config.yml
language:
  - zh-CN
  - en
  - zh-HK
  - zh-TW
```

## 网站标题

```yaml blog/_config.yml
# 网站标题
title: my blog
```

## 网站图标

### 简单方式

```yaml blog/_config.yml
# 网站图标，更多尺寸等图标请使用import方式批量导入
favicon: https://cdn.jsdelivr.net/gh/xaoxuu/assets@master/favicon/favicon.ico
# 作者头像，会出现在文章标题下方，不同于侧边栏的大头像
avatar: https://cdn.jsdelivr.net/gh/xaoxuu/assets@master/avatar/avatar.png
```

### 完全自定义方式

```yaml blog/_config.yml
# 全局导入
import:
  meta:
  - "<meta name='theme-color' content='#FFFFFF'>"
  - "<meta name='msapplication-TileColor' content='#1BC3FB'>"
  - "<meta name='msapplication-config' content='https://cdn.jsdelivr.net/gh/xaoxuu/cdn-favicon@19.9.6/browserconfig.xml'>"
  link:
  - "<link rel='shortcut icon' type='image/x-icon' href='https://cdn.jsdelivr.net/gh/xaoxuu/cdn-favicon@19.9.6/favicon.ico'>"
  - "<link rel='icon' type='image/x-icon' sizes='32x32' href='https://cdn.jsdelivr.net/gh/xaoxuu/cdn-favicon@19.9.6/favicon-32x32.png'>"
  - "<link rel='apple-touch-icon' type='image/png' sizes='180x180' href='https://cdn.jsdelivr.net/gh/xaoxuu/cdn-favicon@19.9.6/apple-touch-icon.png'>"
  - "<link rel='mask-icon' color='#1BC3FB' href='https://cdn.jsdelivr.net/gh/xaoxuu/cdn-favicon@19.9.6/safari-pinned-tab.svg'>"
  - "<link rel='manifest' href='https://cdn.jsdelivr.net/gh/xaoxuu/cdn-favicon@19.9.6/site.webmanifest'>"
  # script:
```


## 设置网站页脚

```yaml blog/_config.yml
# 网页最底部的文字，支持md
copyright: '[Copyright © 2017-2020 Mr. X](https://xaoxuu.com)'
```

## Import

可以在无需修改主题文件的情况下在head和body中添加各种标签。`meta` 和 `link` 对应head中的 `<meta>` 和 `<link>` 标签。`script` 可以在body末尾导入js文件。

```yaml blog/_config.yml
# 全局导入
import:
  meta:
  - "<meta name='theme-color' content='#FFFFFF'>"
  - "<meta name='msapplication-TileColor' content='#1BC3FB'>"
  - "<meta name='msapplication-config' content='https://cdn.jsdelivr.net/gh/xaoxuu/assets@master/favicon/favicons/browserconfig.xml'>"
  link:
  - "<link rel='shortcut icon' type='image/x-icon' href='https://cdn.jsdelivr.net/gh/xaoxuu/assets@master/favicon/favicon.ico'>"
  - "<link rel='icon' type='image/x-icon' sizes='32x32' href='https://cdn.jsdelivr.net/gh/xaoxuu/assets@master/favicon/favicons/favicon-32x32.png'>"
  - "<link rel='apple-touch-icon' type='image/png' sizes='180x180' href='https://cdn.jsdelivr.net/gh/xaoxuu/assets@master/favicon/favicons/apple-touch-icon.png'>"
  - "<link rel='mask-icon' color='#1BC3FB' href='https://cdn.jsdelivr.net/gh/xaoxuu/assets@master/favicon/favicons/safari-pinned-tab.svg'>"
  - "<link rel='manifest' href='https://cdn.jsdelivr.net/gh/xaoxuu/assets@master/favicon/favicons/site.webmanifest'>"
  # script:
```

## 更多配置

更多请见Hexo官方文档：[#Hexo配置](https://hexo.io/zh-cn/docs/configuration)
