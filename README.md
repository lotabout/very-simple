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
menu:
  Home: /
  Archives: archives
social:
    rss: /atom.xml
fancybox: false
duoshuo: #duoshuo_shortname
disqus: #disqus _shortname
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

##Features

#### Pages

To customize pages, such as traditional 'About' page, just create a new page
`about.md` in `/source`, and then add link to the page to `menu` configuration that
we described in previous section.

#### Excerpt
You can control the abstract of a post shown at index, by either filling a
`description:` item in `front-matter` of the `post.md`, or just inserting a
`<!--more-->` before your hidden content.

Otherwise it will fetch the first paragraph as excerpt.
