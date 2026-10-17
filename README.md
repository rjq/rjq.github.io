# RJQ website

Personal site built with [Jekyll](https://jekyllrb.com) and the [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) theme, deployed to GitHub Pages by `.github/workflows/pages-deploy.yml`.

## Local development

Chirpy needs Ruby 3.x (it does not support Ruby 4). With Homebrew's `ruby@3.4`:

```bash
export PATH="/opt/homebrew/opt/ruby@3.4/bin:$PATH"
bundle install
bundle exec jekyll serve --livereload   # http://127.0.0.1:4000
```

If native gems fail to compile with a `tapi error: malformed file` linker error, your selected Xcode is older than the installed macOS SDK. Prefix the install with `DEVELOPER_DIR=/Library/Developer/CommandLineTools`.

## Branding

| File | Purpose |
| --- | --- |
| `assets/css/jekyll-theme-chirpy.scss` | Brand palette (dark theme), fonts, chromatic-aberration title treatment |
| `_data/origin/cors.yml` | Loads Montserrat + Source Sans 3 from Google Fonts |
| `assets/img/avatar.webp` | Sidebar avatar |
| `assets/img/rjq-wordmark.svg` | Vector wordmark (use `<img class="rjq-wordmark" ...>`) |
| `assets/img/social-preview.jpg` | Default link-preview image |
| `assets/img/favicons/` | Favicons and PWA icons |

## Writing

Add posts to `_posts/` as `YYYY-MM-DD-title.md`. See the [Chirpy docs](https://chirpy.cotes.page/posts/write-a-new-post/).
