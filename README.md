# Extreme High School — website

Static site for Extreme High School, Namayumba, built for GitHub Pages. Plain HTML/CSS/JS — no build step.

## Structure

```
index.html      Home
about.html      About / history / mission
fees.html       Fees structure (placeholder figures — replace before publishing)
clubs.html      Clubs & co-curricular life
gallery.html    Photo gallery (placeholder illustrations — swap for real photos)
contact.html    Contact form + map + details
css/style.css   Shared design system
js/main.js      Mobile nav toggle + contact form handling
```

## Before you publish

- **Fees**: `fees.html` has illustrative numbers. Replace with the bursar's actual, current figures.
- **Gallery**: `gallery.html` uses SVG placeholder tiles standing in for real photos. Drop real images into `assets/images/`, then replace each `<svg>...</svg>` block with `<img src="assets/images/your-photo.jpg" alt="…">`, keeping the same `.gallery-cap` caption underneath.
- **Contact form**: GitHub Pages can't run server code, so the form currently just confirms locally in the browser (see `js/main.js`) instead of actually emailing anyone. Wire it up to a free form backend like Formspree or FormSubmit (add their `action` URL to the `<form>` tag) if you want messages to actually arrive by email.
- **Contact details / phone numbers / email**: update the placeholders in the footer and on `contact.html` with the school's real, current contact information.
- **Map**: the embed on `contact.html` currently points to a generic "Namayumba, Uganda" search. Swap in the exact school address or Google Maps place link for a precise pin.

## Publishing to GitHub Pages

1. Push these files to the root of your `extreme-high-school` repo (replacing what's there).
2. In the repo's Settings → Pages, set the source to the branch you pushed to (root folder).
3. The site will be live at `https://<your-username>.github.io/extreme-high-school/`.
