# Webmention Analytics

An analytics dashboard for webmention.io data.

## Features

* Group data by month
* Overview of incoming webmentions by day
* Support for 5 types of webmentions (likes, replies, reposts, mentions, bookmarks)
* Top sources sending webmentions to your site
* Top targets on your site receiving webmentions
* Top tweets generating webmentions through brid.gy
* Webmentions flagged as spam (domains on a blocklist)
* Automatic daily updates

**Attention:**
**This fork has changed the output folder from ``/dist`` to ``/docs`` in order to publish the code to Github Pages!**

## Get your own instance

Things you may need:

* a Github account
* a site registered on [webmention.io](https://webmention.io)
* backfeed of Twitter via [brid.gy](https://brid.gy) (optional)

The easiest way to get started is to fork this repo and deploy it to a Github Page. Find out more on this here:

[Deploy to Github Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)

### 1. Edit Settings

Open `src/data/meta.json` and edit it to fit your site. Adjust the `url` to the URL of the Github Page where the code will be deployed, the `domain` to match the domain of your webmention.io account and the `theme` you want to use by default (dark or light)

### 2. Set Webmention Token

To fetch webmention.io data, you need to set a new **environment variable** called `WEBMENTION_IO_TOKEN`. You can find this token on your webmention.io [settings page](https://webmention.io/settings) under "API Key".
