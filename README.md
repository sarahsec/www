# Sarah Maia Portfolio (Ruby/Jekyll)

A fully Ruby-powered portfolio using Jekyll (GitHub Pages friendly), with content managed via Jekyll data files and Liquid templates.

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

## Personalization

- Main contact email: `hi@sarahmaia.eu.org`
- Update social links in `_data/profile.yml`.
