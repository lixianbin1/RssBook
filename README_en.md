# RssBook

This is a customized RSS reading repository created by osmosfeed.

[中文](./README.md)

### What is RSS?

RSS is a kind of promotion technology originated from Netscape, which transmits the content of users' subscription to their communication collaboration format. RSS builds a technical platform for the rapid dissemination of information, making everyone a potential information provider; From the RSS reader's point of view, it is not necessary to consider what it really means, as long as it is simply understood as a convenient information acquisition tool; The main versions are 0.91, 1.0, 2.0

### The origin of RSS

1997 - Dave winer developed scriptingnews. RSS was born.

1999 - Netscape developed RSS 0.90 (supported by scripting News). This is simple XML with an RDF header.

2000 - userland released the formal 0.91 specification

2003 - the official RSS 2.0 specification was released.

### The fall of RSS?

In 2013, as Google announced the closure of RSS subscription service Google Reader; Domestic websites have shut down RSS subscription services;

At present, only a small number of websites or private RSS services are left;

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
