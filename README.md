# Sarah Maia Portfolio (Ruby/Jekyll)

A fully Ruby-powered portfolio using Jekyll, prepared for GitHub Pages.

## Project structure

- `index.md`: homepage template rendered by Jekyll
- `_layouts/default.html`: shared site layout
- `_data/profile.yml`: profile content (bio, education, links, contact email)
- `assets/css/style.css`: visual styling

## Run locally

```bash
bundle install
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000`.

## Publish on GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select your branch (for example, `main`) and folder `/ (root)`.
5. Save.

## About GitHub's "adding a theme" docs

This portfolio uses a **custom visual theme** (custom layout + custom CSS), so `theme` is intentionally set to `null` in `_config.yml`.

If you want to switch to a built-in GitHub Pages theme from the docs workflow, set a supported value like:

```yml
theme: minima
```

and remove/adjust custom layout/styles as needed.

## Personalization

- Main contact email: `hi@sarahmaia.eu.org`
- Update social links in `_data/profile.yml`.
