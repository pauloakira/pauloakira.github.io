# pauloakira.github.io

Personal academic site, built on the [academicpages](https://github.com/academicpages/academicpages.github.io)
Jekyll template (a fork of [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)).

Live at: https://pauloakira.github.io

## Editing content

| Section        | Where                                       |
| -------------- | ------------------------------------------- |
| Bio / About    | `_pages/about.md`                           |
| CV             | `_pages/cv.md` (and PDF in `files/cv.pdf`)  |
| Publications   | `_publications/YYYY-MM-DD-slug.md`          |
| Projects       | `_portfolio/slug.md`                        |
| Sidebar / nav  | `_config.yml` (`author:`) and `_data/navigation.yml` |
| Profile photo  | `images/profile.png`                        |

Each publication or project is its own markdown file with YAML frontmatter — see
the existing examples in `_publications/` and `_portfolio/` for the schema.

## Local preview

Requires Ruby (any 3.x) and Bundler.

```sh
bundle install
bundle exec jekyll serve --livereload
```

The site will be served at <http://localhost:4000>.

## Deploying

Pushing to `main` triggers a GitHub Pages build automatically. Make sure
**Settings → Pages → Build and deployment → Source** is set to **Deploy from a
branch**, branch `main`, folder `/ (root)`.
