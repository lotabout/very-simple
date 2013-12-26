# Hexo Theme Unit Test

This is a dummy Hexo site for theme unit test. You should test your theme before release.

This test doesn't contain the default theme. You have to install the theme you want to test before starting.

## Usage

1. Clone this repository

    ``` bash
    $ git clone https://github.com/tommy351/hexo-theme-unit-test.git
    ```

2. Install your own theme and modify `theme` setting in `_config.yml`.
3. Run server and start testing. Make sure all styles  are displayed properly.
4. Once test is done, you can [submit your theme](https://github.com/tommy351/hexo/wiki/Themes)!

## Checklist

### `<head>`

- Use the proper [DOCTYPE](https://en.wikipedia.org/wiki/Document_Type_Declaration). If you don't know which doctype you should use, `<!DOCTYPE html>` is recommended.
- UTF8 charset

    ``` html
    <meta charset="utf-8">
    ```

- Proper titles for different pages
- RSS support

    ``` html
    <link rel="alternative" href="path/of/rss" type="application/atom+xml">
    ```

- Favicon support

    ``` html
    <link rel="icon" href="path/of/favicon">
    ```

### Index

- Only display excerpts. (Better with a "Read More" link)
- [Pagination](http://zespia.tw/hexo/docs/pagination.html)

### Post

- Display post categories and tags.
- Disqus comment support.
- Display the post date.
- Support `photo` and `link` layout.
- Posts without title should be accessible.

### Optional

- Responsive design
- i18n
- Post share
- SEO

## Resources

- [Theme](http://zespia.tw/hexo/docs/themes.html)
- [Variables](http://zespia.tw/hexo/docs/variables.html)
- [Helpers](http://zespia.tw/hexo/docs/helpers.html)