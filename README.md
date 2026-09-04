# The Slow Mend — starter site

A 3-page static site: Home, Insights, Contact us. No build tools, no framework — just HTML, CSS, and a little JS for the mobile menu.

## Files

- `index.html` — Home
- `insights.html` — full post list
- `contact.html` — contact form
- `styles.css` — all styling
- `script.js` — mobile nav toggle

## Personalize it before you publish

- Swap the placeholder posts for your own writing (in `index.html` and `insights.html`).
- Replace `hello@theslowmend.com` in `contact.html` with your real email.
- Change "The Slow Mend" to your own blog name if you'd like (search and replace across all three HTML files).
- Add a real photo of yourself or a header image if you want one — none is included by default, to keep the download copyright-clean. Drop an `<img>` tag into the hero section in `index.html`.

## Host it for free

Two easy options:

**GitHub Pages**
1. Create a free GitHub account and a new repository.
2. Upload all the files in this folder to the repository (drag and drop works, or use `git push`).
3. In the repo, go to Settings → Pages, set the source branch to `main` and the folder to `/root`.
4. Your site will be live at `https://yourusername.github.io/repo-name/` within a few minutes.

**Netlify**
1. Create a free Netlify account.
2. Drag this whole folder onto the "Deploy manually" area on your Netlify dashboard.
3. Netlify gives you a free `.netlify.app` URL instantly; you can rename it or connect a custom domain later.

Both are free with no credit card required for a personal blog at this scale.

## Making the contact form actually send email

Static hosting (GitHub Pages, Netlify) can't process form submissions on its own. The easiest free fix:

1. Sign up at [formspree.io](https://formspree.io) (free tier: 50 submissions/month).
2. Create a new form and copy the endpoint it gives you, something like `https://formspree.io/f/abc123`.
3. In `contact.html`, replace `https://formspree.io/f/your-form-id` in the `<form action="...">` tag with your real endpoint.

That's it — submissions will land in your email.

## Adding new blog posts

There's no CMS here; each post is just a block of HTML. To add one:
1. Copy an existing `<article class="post-entry">...</article>` block in `insights.html`.
2. Update the tag class (`tag--sciatica`, `tag--muscle`, or `tag--anxiety`), title, date, and excerpt.
3. Optionally add the same entry to the "Latest insights" section on `index.html` so new posts show on the homepage too.

If you outgrow copy-pasting HTML, a free static site generator like Eleventy or Hugo (or moving to a platform like WordPress.com) would let you write posts in Markdown instead — happy to help you migrate when you're ready.
