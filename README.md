# Academic Portfolio Website (Jekyll + GitHub Pages)

A modern, minimal, and maintainable portfolio site designed for fully funded PhD applications in the USA.

## Included sections

- About me
- Projects
- Publications
- Blog
- Work experience

All content sections are maintained with Markdown.

## Tech stack

- **Jekyll** (stable static site generator with long-term GitHub support)
- **GitHub Pages + GitHub Actions** for CI/CD deployment
- **Markdown collections** for easy editing and extension

## Quick start

### 1) Install dependencies

```bash
bundle install
```

### 2) Run locally

```bash
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000`.

## Content management (Markdown-first)

- Home page sections: `index.md`
- Projects: `_projects/*.md`
- Publications: `_publications/*.md`
- Work experience: `_experience/*.md`
- Blog posts: `_posts/*.md`

You can add, remove, or edit markdown files without touching templates.

## SEO features included

- `jekyll-seo-tag` for metadata, Open Graph, and structured defaults
- `jekyll-sitemap` for automatic sitemap generation
- `robots.txt` included
- Clean URLs and semantic heading structure

## Deployment (CI/CD)

A workflow is included at `.github/workflows/deploy.yml`.

1. Push to `main` (or `master`).
2. GitHub Action builds and deploys automatically.
3. Enable **Pages** in repository settings using **GitHub Actions** as source.

## Customization checklist

- Update identity values in `_config.yml`
- Replace placeholder content in all markdown files
- Add your Google Scholar / ORCID links
- Add a custom domain (optional)

## License

MIT (`LICENSE`).
