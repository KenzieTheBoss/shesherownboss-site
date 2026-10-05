# She's Her Own Boss

The website for She's Her Own Boss — shesherownboss.com

## What's here

- `public/index.html` — the main site
- `public/journal.html` — The Journal
- `public/og-image.png` — the link preview card

## Editing

Change the files in `public/`. Cloudflare redeploys automatically when this
repo is pushed to.

## Forms

Both the Work With Me form and the newsletter signup read their endpoints from
a settings block near the top of each page's script:

```js
var FORM_ENDPOINTS = { contact: '', newsletter: '' };
```

Paste Formspree endpoints between the quotes and the forms start working. Left
blank, visitors are shown an email address instead of the form silently failing.
