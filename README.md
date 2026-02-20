# Sarah Maia Portfolio (Ruby/Jekyll)

A fully Ruby-powered portfolio using Jekyll, now prepared for both GitHub Pages and Vercel.

## Project structure

- `index.md`: homepage template rendered by Jekyll
- `_layouts/default.html`: shared site layout
- `_data/profile.yml`: profile content (bio, experience, education, skills, links, contact)
- `assets/css/style.css`: visual styling
- `vercel.json`: Vercel build/output configuration

## Run locally

```bash
bundle install
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000`.

## Deploy on Vercel

1. Import this repository into Vercel.
2. Framework preset: **Other** (or let Vercel auto-detect with `vercel.json`).
3. Build command: `bundle exec jekyll build`.
4. Output directory: `_site`.

These settings are already defined in `vercel.json`.

### Ruby runtime note

> "The Ruby runtime takes in a Ruby program that defines a singular HTTP handler and outputs it as a Vercel Function."

This portfolio is static by default, but you can add Ruby serverless routes if you later need dynamic endpoints.

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
- Update sections and social links in `_data/profile.yml`.
