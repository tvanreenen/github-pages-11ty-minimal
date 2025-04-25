# Minimal Eleventy Blog Template

A minimal, opinionated template for creating a blog with [Eleventy](https://www.11ty.dev/) and deploying to GitHub Pages.

## Features

- 🚀 Simple setup with minimal dependencies
- 📝 Markdown-based blog posts
- 🌓 Automatic light/dark mode support with [Simple.css](https://simplecss.org)
- 🎨 Clean, readable typography and layout
- 🔄 Automatic GitHub Pages deployment
- 📱 Responsive design

## Getting Started

1. Click "Use this template" to create a new repository
2. Clone your new repository
3. Create your first post in `posts/article-title/index.md`
4. Test locally with `npx @11ty/eleventy --serve`
5. Push to GitHub - your site will be automatically built and deployed

## Project Structure

```
.
├── _includes/         # Layout templates
├── posts/            # Blog posts (article-title/index.md)
├── .eleventy.js      # Eleventy configuration
├── .github/          # GitHub Actions workflow
└── index.html        # Homepage
```

## Writing Posts

Create a new post by adding a markdown file at `posts/article-title/index.md`:

```markdown
---
title: "My First Post"
date: 2024-01-01
---

Your post content here...
```

## Customization

- Edit `_includes/layout.html` to modify the site structure
- Posts are organized by article paths/titles in the `posts` directory
- The homepage automatically lists all posts in reverse chronological order

## Deployment

The site is automatically built and deployed to GitHub Pages when you push to the `main` branch.

## Credits

- [Eleventy](https://www.11ty.dev/) - Static site generator
- [Simple.css](https://simplecss.org) - Minimal CSS framework
- [GitHub Pages](https://pages.github.com/) - Hosting

## License

MIT

---

For a more feature-rich Eleventy blog template, check out [eleventy-base-blog](https://github.com/11ty/eleventy-base-blog).