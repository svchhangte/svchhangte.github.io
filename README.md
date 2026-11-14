# SV Chhangte — Jekyll blog

A lightweight, text-focused personal blog for GitHub Pages.

## 1. Create the GitHub repository

1. Sign in to GitHub.
2. Create a **public** repository named exactly `YOUR-USERNAME.github.io`.
3. Upload the contents of this project to the repository root (not the containing folder).
4. Commit the files to the `main` branch.

Your free site address will be `https://YOUR-USERNAME.github.io/`.

## 2. Set the site URL

Open `_config.yml` and replace:

```yml
url: "https://YOUR-USERNAME.github.io"
```

with your real GitHub Pages address. Keep `baseurl: ""` for a username site repository.

Also replace the `YOUR-USERNAME` placeholder in this README if you keep it in your repository.

## 3. Enable GitHub Pages

1. Open the repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **GitHub Actions** as the source.
3. Open the **Actions** tab and wait for the Pages workflow to finish.
4. Visit `https://YOUR-USERNAME.github.io/`.

The included workflow builds and deploys the Jekyll site whenever you push to `main`.

## 4. Publish a post

Create a Markdown file in `_posts/` using this naming pattern:

`YYYY-MM-DD-your-post-title.md`

Example:

```markdown
---
title: "The Art of Reading Slowly"
date: 2026-11-14
categories: [Books, Reflections]
description: "A few thoughts on reading with patience."
---

Write your article here in Markdown.

## A section heading

Your paragraphs go here.
```

Commit the file to `main`. GitHub Actions will rebuild the site. The post URL will be `/the-art-of-reading-slowly/`.

## 5. Edit your pages

- `about.md` — About page
- `bookshelf.md` — Bookshelf
- `archive.md` — Chronological archive
- `index.html` — Homepage introduction
- `assets/css/style.css` — All visual styling
- `_config.yml` — Site title, description, URL and settings

## 6. Search engines

The project includes:
- `jekyll-seo-tag` for page metadata
- `jekyll-sitemap` for an XML sitemap
- `jekyll-feed` for RSS
- `robots.txt` pointing crawlers to the sitemap

After deployment:
1. Open Google Search Console and add your `https://YOUR-USERNAME.github.io/` property.
2. Verify ownership using one of the methods Google offers.
3. Submit `sitemap.xml`.
4. Use URL Inspection to request indexing of your homepage and important articles.

Indexing is not guaranteed. Google decides which pages to index and when.

## 7. Important migration note

Do not delete your Bear Blog or stop renewing it until you have:
- copied all your articles, images and metadata;
- checked that every migrated article works;
- deployed and tested the new site;
- decided how to handle old Bear Blog URLs.

If your old Bear Blog URLs differ from the new URLs, permanent redirects are ideal. Do not assume that simply publishing the same article at a new address transfers its search visibility.

## Notes

- GitHub Pages is free for public repositories on GitHub Free.
- This project uses GitHub Actions for deployment.
- The starter post is an example; replace it with your own article or delete it. The bookshelf page contains placeholders for your reading lists.
