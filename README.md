# Vineet J Nair - Personal Website

A clean, simple academic website built with Jekyll and the Minima theme.

## Quick Start

### Local Development

1. Install Ruby and Bundler if you haven't already
2. Clone this repository
3. Install dependencies:
   ```bash
   bundle install
   ```
4. Run the local server:
   ```bash
   bundle exec jekyll serve
   ```
5. Visit `http://localhost:4000` in your browser

### GitHub Pages Deployment

1. Create a new repository named `vineetjnair9.github.io` (or use your existing one)
2. Push this code to the repository
3. Go to Settings > Pages
4. Set Source to "Deploy from a branch"
5. Select the `main` branch (or `master` if that's your default)
6. Save and wait a few minutes for deployment

Your site will be live at `https://vineetjnair9.github.io`

## File Structure

```
.
├── _config.yml          # Site configuration
├── Gemfile              # Ruby dependencies
├── index.md             # Homepage
├── about.md             # About page
├── publications.md      # Publications page
├── cv.md               # CV page
└── _posts/             # Blog posts (optional)
```

## Customization

### Adding Content

- **Homepage**: Edit `index.md`
- **About**: Edit `about.md`
- **Publications**: Edit `publications.md` - just add your papers in markdown format
- **CV**: Edit `cv.md`

### Blog Posts (Optional)

Create files in `_posts/` with the format: `YYYY-MM-DD-title.md`

Example: `_posts/2025-01-10-my-first-post.md`

```markdown
---
layout: post
title: "My First Post"
date: 2025-01-10
categories: research
---

Your content here...
```

### Styling

The Minima theme supports different skins. Change in `_config.yml`:
- `classic` (default)
- `dark`
- `auto` (respects user's system preference)
- `solarized-light`
- `solarized-dark`

### Adding Your Photo

1. Create an `assets` folder
2. Add your photo: `assets/profile.jpg`
3. Reference it in your pages using: `![Photo](/assets/profile.jpg)`

## No More CSV Files!

With this setup, you just edit markdown files directly. No more dealing with CSV files for publications - just add them as formatted text in `publications.md`.

## Support

For Jekyll documentation: https://jekyllrb.com/docs/
For Minima theme: https://github.com/jekyll/minima
