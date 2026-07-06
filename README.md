# mikaylin.co.za

Mikaylin's personal site — football, photography, and gaming, plus a blog.

## Pages

- `/` — Landing page
- `/about/` — About
- `/photography/` — Photography gallery + posts
- `/football/` — Football stats + posts
- `/gaming/` — Gaming stats + posts
- `/blog/` — All blog posts, filterable by category

## Adding a blog post

Create a new Markdown file in `src/content/posts/`, e.g. `src/content/posts/my-new-post.md`:

```md
---
title: "Your post title"
description: "One sentence summary shown on post cards."
category: "football" # one of: football, photography, gaming, life
pubDate: 2026-07-10
---

Write your post here using normal Markdown — paragraphs, **bold**, lists, etc.
```

The post automatically shows up on `/blog/` and on its category page (e.g. a `football` post appears on `/football/`), sorted newest first. Set `draft: true` in the frontmatter to hide a post while you're still writing it.

## Adding a photo to the gallery

Drop an image file into `src/assets/gallery/` and it will automatically appear in the gallery on `/photography/`. Prefix filenames with numbers (e.g. `01-`, `02-`) to control the order.

## Commands

| Command             | Action                                      |
| :------------------- | :------------------------------------------ |
| `npm install`        | Install dependencies                        |
| `npm run dev`        | Start local dev server at `localhost:4321`  |
| `npm run build`      | Build the production site to `./dist/`      |
| `npm run preview`    | Preview the production build locally        |

Full Astro documentation: https://docs.astro.build
