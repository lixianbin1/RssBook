# RssBook

This is a customized RSS reading repository created by osmosfeed.

[中文](./README.md)

### Customize the feed

1. In the repository root, open `osmosfeed.yaml` file, click the "Pencil (Edit this file)" button to edit.
2. Remove `# ` to uncommend the `cacheUrl` property, replace `<github_username>` with your GitHub username, and replace `<repo>` with your GitHub repo name.
3. In the sources, update the items to the sources you want to follow. The final content of the file should look similar to this:

   ```yaml
   cacheUrl: https://<github_username>.github.io/<repo>/cache.json
   sources:
     - href: https://my-rss-source-1/feed/
     - href: https://my-rss-source-2/rss/
     - href: https://my-rss-source-3/feed
     - href: https://my-rss-source-4/news/rss
     - href: https://my-rss-source-5/rss/
   ```

4. Scroll to the bottom of the page, click "Commit changes" button.
5. Once the rebuild finishes, your feed will be available at `https://<github_username>.github.io/<repo>`.

## Links and references

- [How does it work?](https://github.com/osmoscraft/osmosfeed#osmosfeed)
- [File an issue about the template](https://github.com/osmoscraft/osmosfeed-template)
- [File an issue about the tool](https://github.com/osmoscraft/osmosfeed)
- [Lastest documentation](https://github.com/osmoscraft/osmosfeed)
