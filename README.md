# Ayu Larasati — UX Research Portfolio

Personal portfolio site for Francine Goulde, Senior UX Researcher. Built with plain HTML, CSS, and vanilla JavaScript — no frameworks, no dependencies, no build step.

**Live site:** [a-larasati.github.io](https://a-larasati.github.io/uxr-portfolio/)

---

## Files

```
index.html          Main portfolio (hero, about, case study cards, resume, contact)
case-study-1.html   Case Study 01 — ATS Discovery & Evaluation (password protected)
case-study-2.html   Case Study 02 — Platform Redesign Evaluation (password protected)
README.md           This file
```

---

## Updating content

### Swap in your photos
Both image placeholders are clearly marked in the HTML with comments. Find the relevant `div` and replace it with a standard `img` tag:

```html
<!-- Before -->
<div class="profile-photo-placeholder"> ... </div>

<!-- After -->
<img src="profile.jpg" alt="Francine Goulde" style="width:220px;height:220px;border-radius:50%;object-fit:cover;" />
```

Add your image files to the same folder as the HTML files, then reference them by filename.

### Change the case study password
Both case study pages use the same password. Open `case-study-1.html` and `case-study-2.html`, find this line near the bottom of each file, and update the value:

```js
const PASSWORD = "research2026";
```

### Update your LinkedIn URL
In `index.html`, find the LinkedIn link in the contact section and replace the `href`:

```html
<a href="https://www.linkedin.com/in/your-actual-profile" ...>
```

### Update text content
All content is plain HTML — no CMS, no special syntax. Open any file in a text editor and edit directly.

---

## Deploying updates

After making changes, commit and push to the `main` branch. GitHub Pages will automatically rebuild and publish within a minute or two.

If you're editing through the GitHub browser UI: click the file → click the pencil icon to edit → commit changes directly.

---

## Design notes

- **Colors:** Soft lavender, cream, yellow, and orange — pulled from the original case study presentation
- **Fonts:** [Fraunces](https://fonts.google.com/specimen/Fraunces) (display) + [DM Sans](https://fonts.google.com/specimen/DM+Sans) (body) via Google Fonts
- **Password protection:** Client-side only — suitable for keeping casual visitors out, not for highly sensitive content
- **No frameworks or build tools** — every file works by opening it directly in a browser
