# RssBook

[English](./README_en.md)

这是一个通过osmosfeed创建的私人定制的RSS阅读的存储库.[已停止RSS推送]

### 什么是RSS?

RSS是一种起源于网景的推广技术，将用户订阅的内容传送给他们的通讯协同格式。RSS搭建了信息迅速传播的一个技术平台，使得每个人都成为潜在的信息提供者;如果从RSS阅读者的角度来看，完全不必考虑它到底是什么意思，只要简单地理解为一种方便的信息获取工具就可以了；主要的版本有0.91, 1.0, 2.0

### RSS的起源

1997 年 - Dave Winer 开发出 scriptingNews。RSS 由此诞生。

1999 年 - Netscape 开发出 RSS 0.90 （由 scriptingNews 支持的）。这是带有一个 RDF header 的简单的 XML。

2000 年 - UserLand 发布了正式的 0.91 规范

2003 年 - 正式的 RSS 2.0 规范发布。

### RSS的陨落？

2013 年，随着谷歌宣布关闭闭RSS订阅服务Google Reader；国内网站先后关闭RSS订阅服务；
目前只剩下小部分网站或者私人转发的rss服务；

### 配置订阅

1. 进入仓库的根目录，打开`osmosfeed.yaml`文件, 单击有铅笔图标的Edit this file（编辑此文件）按钮。
2. 删除 `# ` 从而取消`cacheUrl`一行的注释。将`<github_username>`替换为GitHub用户名，将`<repo>`替换为仓库名.
3. 在`sources:`(订阅源)下，添加你想要的RSS/Atom源。

   ```yaml
   cacheUrl: https://<github_username>.github.io/<repo>/cache.json
   sources:
     - href: https://my-rss-source-1/feed/
     - href: https://my-rss-source-2/rss/
     - href: https://my-rss-source-3/feed
     - href: https://my-rss-source-4/news/rss
     - href: https://my-rss-source-5/rss/
   ```

4. 单击页面底部的Commit changes（提交更改）按钮。
5. 等待前端自动静态生成（1－3分钟）。阅读器将在`https://<github_username>.github.io/<repo>`接受访问。

## 链接和引用

- [它是怎么工作的](https://github.com/osmoscraft/osmosfeed#osmosfeed)
- [提交有关模板的问题](https://github.com/osmoscraft/osmosfeed-template)
- [提出有关该工具的问题](https://github.com/osmoscraft/osmosfeed)
- [上次测试文档](https://github.com/osmoscraft/osmosfeed)
