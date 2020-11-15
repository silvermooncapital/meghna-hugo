# Silver Moon Capital Website

## Basics

- GitHub location: https://github.com/silvermooncapital/meghna-hugo
- Forked from [meghna-hugo](https://github.com/themefisher/meghna-hugo).
- Built with the static website generator [Hugo](https://gohugo.io).

## Blog Section

Currently disabled. To re-enable:

- Uncomment the blog partial in `layouts/index.html`:

    ```
    {{ partial "blog.html" . }}
    ```

- Uncomment the link to the blog section in the menu header in `exampleSite/config.toml`:

    ```
    [[menu.main]]
    name = "blog"
    pre = "#"
    url = "blog"
    weight = 2
    ```

- Place blog articles in `exampleSite/content/english/blog` as Markdown files. (See `simple-blog-post-1.md` as an example.)
- Place images associated with blog posts in `exampleSite/static/images/blog`.