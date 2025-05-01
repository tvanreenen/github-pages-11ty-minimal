# Minimal Static Site Blog Template

A minimal, opinionated template for creating a blog using [Eleventy](https://www.11ty.dev/) as the static site generator and deploying to [GitHub Page](https://pages.github.com/) or [Cloudflare Pages](https://pages.cloudflare.com/).

## Getting Started

1. Click "Use this template" to create a new repository
2. Clone your new repository
3. Create your first post in `posts/post-title/index.md`
4. Test locally with `npx @11ty/eleventy --serve`
5. Push to GitHub - your site will be automatically built and deployed

## Project Structure

```
.
├── _includes/        # Layout templates
├── css/              # Custom stylesheets
├── posts/            # Blog posts (post-title/index.md)
├── .eleventy.js      # Eleventy configuration
├── .github/          # GitHub Actions workflow
└── index.html        # Homepage
```

## Writing Posts

This configuration of 11ty is setup as a simple blog roll where each post is self-contained in its own directory (the markdown and any assests). The folder name will be the URL slug (`posts/my-post/index.md` -> `site.com/my-post`). The YAML frontmatter controls the title and any othe details you want to include in the list view. 

```markdown
---
title: "My First Post"
date: 2024-01-01
---

Your post content here...
```

## Customizing

- Include the CSS of your choice directly in the `HEAD` or in the `css/` folder. It should implement the semantic HTML equivalent to markdown using class-less style. Simple.css is included as a starter framework. See the [Simple.css customization guide](https://github.com/kevquirk/simple.css/wiki/Getting-Started-With-Simple.css#customise-simplecss) for more details.
- Customize the site structure by modifying any of the files in `_includes/`.
- Explore Eleventy's many other customization options in their [official documentation](https://www.11ty.dev/docs/)

## Deployment

- To automatically deploy on GitHub Pages
  - Follow https://docs.github.com/en/pages/quickstart
  - Rename `.github/workflows/deploy.yml.example` to `.github/workflows/deploy.yml`
- To deploy to Cloudflare Pages:
  - Follow https://developers.cloudflare.com/pages/get-started/git-integration/
- When you push to the `main` branch, the site will be built in the `_site` directory and deployed automatically.

---

This was inspred by the more feature-rich [11ty/eleventy-base-blog](https://github.com/11ty/eleventy-base-blog), but with a minimal setup in mind.
