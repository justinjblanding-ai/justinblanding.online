# justinblanding.online

Plain HTML + CSS. No build step.

```
index.html              home: hero, story, resume, essays, contact
styles.css              all styling (light + dark mode)
essays/_template.html   copy this to write a new essay
```

## Add an essay

1. Copy `essays/_template.html` to `essays/your-essay-slug.html`.
2. Edit the title, date, summary, and body (the template has numbered comments).
3. In `index.html`, find the `#essays` section: uncomment the `<ul class="essay-list">` block, point the link at your new file, and delete the `<div class="empty">` block.

## Put it on justinblanding.online

The domain currently shows a GoDaddy "Launching Soon" page, and GoDaddy's builder doesn't accept uploaded HTML. The easiest free option:

1. Go to https://app.netlify.com/drop and drag the `site` folder onto the page.
2. In Netlify: Domain management → Add a domain → `justinblanding.online`.
3. Netlify shows the DNS records to add. In GoDaddy: My Products → DNS for justinblanding.online, then add those records (replace the existing A / CNAME for `@` and `www`).
4. HTTPS turns on automatically once DNS updates (minutes to a few hours).

GitHub Pages or Cloudflare Pages work the same way if you'd rather keep it in a Git repo.
