# RssBook

[English](./README_en.md)

这是一个通过osmosfeed创建的私人定制的RSS阅读的存储库.

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
