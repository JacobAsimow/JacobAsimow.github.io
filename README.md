# Portfolio Site

Personal portfolio built with [Jekyll](https://jekyllrb.com/), based on
[msaveski/www_personal](https://github.com/msaveski/www_personal).

## Editing content
Almost everything lives in `_data/` — you rarely need to touch HTML.

| File | What it controls |
|---|---|
| `_data/main_info.yaml` | Name, title, email, photo, social links, resume PDF |
| `_data/projects.yaml` | Project cards on the Projects page |
| `_data/skills.yaml` | Skills section |
| `_data/talks.yaml` | Talks & proceedings page |
| `index.html` | The About page (home) |
| `_projects/*.md` | Detail pages for individual projects |

Images go in `assets/` (profile photo in `assets/profile-pics/`, project
thumbnails in `assets/projects/<name>/`, resume in `assets/cv/`).

### Adding a project page
1. Copy `_projects/jamba-jumble.md` to `_projects/my-project.md` and edit it.
2. Add an entry in `_data/projects.yaml` with `url: "/projects/my-project.html"`.

## Running locally
Requires Ruby 3.x (macOS's system Ruby 2.6 is too old — install with
`brew install ruby` or rbenv).

```sh
bundle install
bundle exec jekyll serve
# open http://localhost:4000
```

## Deploying (GitHub Pages)
1. Push this repo to GitHub. Naming it `<username>.github.io` serves it at
   `https://<username>.github.io` (keep `baseurl: ""`). Any other repo name
   serves at `https://<username>.github.io/<repo>` — set `baseurl: "/<repo>"`
   in `_config.yml`.
2. In the repo: **Settings → Pages → Build from branch → `main` / root**.

## Libraries
Skeleton CSS, Font Awesome 6.6, Academicons, jQuery 3.1.1.
