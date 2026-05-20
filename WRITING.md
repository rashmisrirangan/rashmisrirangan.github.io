# How to Write a New Post

## 1. Create a file in `_posts/`

Name it exactly like this: `YYYY-MM-DD-your-post-title.md`

Examples:
- `_posts/2026-05-20-indoor-air-quality-basics.md`
- `_posts/2026-06-01-chemical-safety-in-the-workplace.md`

## 2. Add front matter at the top

Every post must start with this block (including the `---` lines):

```
---
layout: post
title: "Your Post Title Here"
date: 2026-05-20
categories: [environment, health]
tags: [air quality, workplace safety]
---
```

- `title` — shown on the homepage and at the top of the post
- `date` — controls the sort order on the homepage (newest first)
- `categories` and `tags` — optional, for organization

## 3. Write the post body in Markdown

After the front matter, write your content using Markdown:

```markdown
## Section Heading

Regular paragraph text goes here.

**Bold text**, *italic text*, and [links](https://example.com) work as usual.

## Another Section

More content...
```

## 4. Add an excerpt break (optional)

Add `<!--more-->` after your opening paragraph. Everything before it becomes
the preview snippet shown on the homepage.

## 5. Add images

1. Put the image file in `assets/images/` (e.g., `assets/images/soil-diagram.jpg`)
2. Reference it in your post:

```markdown
![Description of the image](/assets/images/soil-diagram.jpg)
```

## 6. Publish

Commit and push the new file to the `main` branch. GitHub Actions will
automatically build and deploy the site within a minute or two.
