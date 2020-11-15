# Silver Moon Capital Website

## Basics

- GitHub location: https://github.com/silvermooncapital/meghna-hugo
- Forked from [meghna-hugo](https://github.com/themefisher/meghna-hugo).
- Built with the static website generator [Hugo](https://gohugo.io).

## Call to Action Section

Configured in `exampleSite/data/en/cta.yml`.

Depending on whether the background image is light or dark, the CSS class can
be switched between `call-to-action` and `call-to-action-2` in
`layouts/partials/cta.html`:

  ```html
  <section id="cta" class="call-to-action-2 section-sm bg-1 overly" style='background-image: url("{{ .bg_image_webp | absURL }}")'>
  ```

## Blog Section

Currently disabled. To re-enable:

- Uncomment the blog partial in `layouts/index.html`:

    ```
    {{ partial "blog.html" . }}
    ```

- Uncomment the link to the blog section in the menu header in `exampleSite/config.toml`:

    ```toml
    [[menu.main]]
    name = "blog"
    pre = "#"
    url = "blog"
    weight = 2
    ```

- Place blog articles in `exampleSite/content/english/blog` as Markdown files. (See `simple-blog-post-1.md` as an example.)
- Place images associated with blog posts in `exampleSite/static/images/blog`.

## Contact Us Form

Configured in `exampleSite/data/en/contact.yml`. The form makes use of the free
Formspree.io service. Form submissions are automatically emailed to SMC.

Note that a Formspree-branded thank you page is presented upon form submission.
This is the only option for the free plan. Other [plans](https://formspree.io/plans)
are available that allow redirection to a custom thank you page.

## Images

Images used on the site:

- Moon over beach: https://unsplash.com/photos/NcF6MVPW644
- Moon over mountains: https://unsplash.com/photos/6msS8vT5pzw
