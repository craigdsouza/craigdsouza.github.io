# craigdsouza.in

Personal site built with Jekyll, hosted on GitHub Pages. Push to `master` → site rebuilds automatically within ~1 minute.

---

## How to update things

### Add a new writing

Create a file in `_posts/` named `YYYY-MM-DD-your-title.md`:

```markdown
---
layout: post
title: "Your post title"
date: 2026-03-05
tags: [tag1, tag2]
---

Your content here. Write in standard markdown.
```

The date in the filename controls ordering. The post appears automatically on the `/writings` page.

---

### Add a report

Create a file in `_reports/` named `your-report-title.md`:

```markdown
---
layout: default
title: "Report title"
date: 2026-03-05
description: "One line summary shown in the listing."
tags: [tag1, tag2]
---

Report content here.
```

The report appears automatically on the `/reports` page, sorted newest first.

---

### Add a tool

Create a file in `_tools/` named `your-tool-name.md`:

```markdown
---
layout: default
title: "Tool name"
date: 2026-03-05
description: "One line summary shown in the listing."
tags: [tag1, tag2]
---

Description and usage notes.
```

The tool appears automatically on the `/tools` page, sorted newest first.

---

### Edit the About page

Edit `about.md` directly. It's plain markdown.

---

### Edit the home page

Edit `index.html`. The four section links are hardcoded — update the descriptions there as needed.

---

### Unpublish an old post without deleting it

Add `published: false` to the post's front matter:

```markdown
---
published: false
layout: post
title: "..."
---
```

The file stays in the repo but won't appear on the site.

---

### Change the site title, description, or email

Edit `_config.yml`. Changes take effect on the next build.

---

## Structure

```
_posts/        → writings (one .md file per post)
_reports/      → reports (collection)
_tools/        → tools (collection)
_layouts/      → HTML templates (default, post, page)
_includes/     → partials (head, nav, footer)
css/main.css   → all styles
index.html     → home page
writings.html  → auto-lists all posts
reports.md     → reports landing page
tools.md       → tools landing page
about.md       → about page
CNAME          → custom domain (craigdsouza.in)
_config.yml    → site settings
```

---

## License

Content under `_posts/` is available under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Code is under [MIT](LICENSE).
