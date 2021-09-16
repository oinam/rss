# Oinam RSS

[Oinam RSS](https://rss.oinam.com/)

## Anatomy of Bubo Reader

- `src/index.html` - a [Nunjucks](https://mozilla.github.io/nunjucks/) template that lets you change how the feeds are displayed
- `output/style.css` - a CSS file to stylize your feed output
- `src/feeds.json` - a JSON file containing the URLs for various site's feeds separated into categories
- `src/index.js` - the script that loads the feeds and does the actual parsinga and rendering

<a id="updated"></a>
### Keeping Feeds Updated

#### Using Netlify Webhooks

To keep your feeds up to date you'll want to [setup a Build Hook](https://www.netlify.com/docs/webhooks/#incoming-webhooks) for your Netlify site and use another service to ping it every so often to trigger a rebuild. I'd suggest looking into:

- [IFTTT](https://ifttt.com/)
- [Zapier](https://zapier.com/)
- [EasyCron](https://www.easycron.com/)

If you already have a server running Linux and some command-line experience it might be simpler to setup a [cron job](https://en.wikipedia.org/wiki/Cron). 

### Credit (Bubo Reader)

For the original and how to setup your own, please visit [Bubo Reader](https://github.com/georgemandis/bubo-rss).