# justinblanding.online

Plain HTML + CSS. No build step. Hosted on GitHub Pages; every push to `main` goes live in a minute or two.

```
index.html              home: hero, about, essays & speeches, contact
styles.css              all styling (light + dark mode)
writing/                PDFs listed under Essays & speeches
essays/_template.html   copy this to write a web-page essay
```

## Write your bio

In `index.html`, find `<section id="about">` and replace `<p>My bio is coming soon.</p>` with your own paragraphs, one `<p>...</p>` per paragraph.

## Add a PDF essay or speech

1. Upload the PDF into the `writing/` folder (use a short name with dashes, like `my-speech.pdf`).
2. In `index.html`, find `<section id="essays">`, copy one `<li>...</li>` block, and change the link, label, title, and one-line description.

## Add a web-page essay

1. Copy `essays/_template.html` to `essays/your-essay-slug.html` and fill it in (the template has numbered comments).
2. Add an `<li>` for it in the `#essays` list, linking to `essays/your-essay-slug.html`.
