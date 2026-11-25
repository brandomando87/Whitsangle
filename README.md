# Whit's Angle of Life — Photo Journal

A cozy, moonlit photography journal built for Whit.

## Important: GitHub Pages Filename Fix
If you are pushing these files to GitHub Pages (`github.com/brandomando87/Whitsangle`), Git previously tracked `Index.html` and `About.html` with capital letters. GitHub Pages is case-sensitive, so run these commands once inside your local repo folder so every link works online:

```bash
git mv Index.html index.html.tmp && git mv index.html.tmp index.html
git mv About.html about.html.tmp && git mv about.html.tmp about.html
git add .
git commit -m "Fix lowercase filenames and add site polish"
git push
```

## Optional: Custom Logo Image
All pages look for `Wesbitelogo.jpg` in this folder and seamlessly fall back to the built-in circular bridge SVG medallion if it isn't present. If you have a custom circular logo image, save it in this folder as `Wesbitelogo.jpg` and it will appear automatically in every header and footer.

## How to Add New Photos
1. Drop the new `.jpg` photo into this folder.
2. Open `index.html` and find `const journalEntries = [`.
3. Copy one entry block, paste it at the top of the list, and update `id`, `entryNumber`, `title`, `categories` (`'riverfront'`, `'skies'`, or `'street'`), `location`, `url`, and `caption`. The photo count updates automatically!

## How to Activate Social Links Later
Open `socials.html` and follow the short comment right above the 4 social cards to turn any card into a live clickable link.

## Customizing the Hidden Dedication Note
Click **"✦ Made with love for Whit ☾"** at the very bottom of any page to preview the hidden dedication modal. You can personalize the message inside `<div id="gift-note-modal">` in the HTML files anytime.
