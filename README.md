# very-simple

[Demo](http://lotabout.github.io/very-simple/)

A theme that aimed to be very simple, creatd by [lotabout](https://github.com/lotabout)

## Installation

Install theme and renderers:

```
git clone https://github.com/lotabout/very-simple themes/very-simple
npm install hexo-renderer-sass --save
npm install hexo-renderer-jade --save
```

Edit `_config.yml` in hexo root, change `theme` to `very-simple`.

## Configuration
Default config:

```
# very-simple/_config.yml
menu:
  Home: /
  Archives: archives
social:
  email:
  twitter:
  github:
  googleplus:
  rss: /atom.xml
fancybox: true
duoshuo: #duoshuo_shortname
disqus: #disqus _shortname
google_analytics: #Google Analytics Tracking Code
google_adsense_page_level_ads: #Google Adsense Page Level Ads Code
```

- menu - The navigation links on the header
- social - Social icons such as email/github/twitter etc. to show on the footer
  - email - Email address
  - twitter - twitter account
  - github - github account
  - googleplus - Google Plus account
  - rss - RSS subscription link, learn more in [hexo-generator-feed](https://github.com/hexojs/hexo-generator-feed)
- fancybox - Enable [Fancybox](http://fancyapps.com/fancybox/)
- duoshuo - [Duoshuo](http://duoshuo.com) shortname
- disqus - [Disqus](https://disqus.com) shortname
- google_analytics - Google Analytics Tracking Code
- google_adsense_page_level_ads: - Google Adsense Page Level Ads Code

If you want to contain this theme only as a submodule, then you may be
unwilling to keep all configuration inside theme
folder(`very-simple/_config.yml`). In this case, you can keep the
configurations in root configuration file `/_config.yml` by:

```
# /_config.yml
very_simple:
  menu:
    Home: /
    Archives: archives
  social:
    email:
    twitter:
    github:
    googleplus:
    rss: /atom.xml
  fancybox: true
  duoshuo: #duoshuo_shortname
  disqus: #disqus _shortname
  google_analytics: #Google Analytics Tracking Code
  google_adsense_page_level_ads: #Google Adsense Page Level Ads Code
```

##Features

#### Logo
You can set a **favicon.ico** for your website, please put it into  `source` folder of hexo directory, recommended size: 32px*32px.

#### Pages

To customize pages, such as traditional 'About' page, follow the following
steps:

1. create a directory `about/` under `/source`
2. create a corresponding index page `index.md` under directory `about/`.
3. add link to the page to `menu` configuration:

    menu:
      About: about

Note that you don't need to add directory and create `about.md` under
`/source`. But the configuration should changed to:

```
    menu:
      About: about.html
```

#### Comments

You can control whether to show comment system(default to enabled) in pages.
Just add `comments: true` or `comments: false` in `front-matter` section of
page. i.e.

```
title: About
date: 2013-12-26 22:52:56
layout: page
comments: true
---
```

#### Excerpt
You can control the abstract of a post shown at index, by:

1. Filling a `description:` item in `front-matter` of the `post.md`
2. Just inserting a `<!--more-->` before your hidden content.
3. Otherwise it will fetch the first paragraph as excerpt.
