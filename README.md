# Mehdi Hellou: academic website

Source for <https://mehdi-hellou.github.io>, built with Jekyll on the
[academic-website-template](https://github.com/sbryngelson/academic-website-template)
by Spencer Bryngelson (MIT licence, see `LICENSE`).

## Where things live

| To change...            | Edit                                              |
|-------------------------|---------------------------------------------------|
| Name, links, nav, theme | `_config.yml`                                     |
| Home page text          | `_pages/home.md`                                  |
| About page              | `_pages/about.md`, `_data/pi.yml` (education)     |
| Research cards          | `_pages/research.md`                              |
| Project detail pages    | `_pages/research-*.md` (URLs kept: `/researches/*.html`) |
| Publications            | `assets/ref.bib` (search for `TODO`)              |
| News (sidebar)          | `_data/news.yml` (the News card appears once it has entries) |
| Photo                   | `images/` and `photo:` in `_config.yml`           |

## Preview locally

```bash
bundle install
bundle exec jekyll serve   # http://localhost:4000
```

## Deploy

Pushing to `main` runs `.github/workflows/deploy.yml`. One-time setting:
**Settings > Pages > Source > "GitHub Actions"**.
