# BUILTVITZ Site Setup

## 1. Add your logo
Save your BUILTVITZ logo (PNG with transparent background recommended) to:
```
images/logo.png
```
The site will automatically use it. If the file is missing, the text wordmark shows as a fallback.

## 2. Add project photos
Drop 6 JPG photos into `images/` named:
- `project-1.jpg` — Modern Residential Build
- `project-2.jpg` — Custom Deck & Stairs
- `project-3.jpg` — Backyard Shed Build
- `project-4.jpg` — Walkway & Hardscape
- `project-5.jpg` — Interior Remodel
- `project-6.jpg` — Outdoor Living Project

Recommended size: ~1200×900px, under 300KB each. The captions in `index.html` can be edited to match your actual projects.

## 3. Wire up the contact form (Formspree)
1. Sign up free at https://formspree.io
2. Create a new form, copy the form ID (looks like `xyzabcde`)
3. In `index.html`, find this line:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST"
   ```
4. Replace `YOUR_FORM_ID` with your actual Formspree ID. Submissions will email you.

Free tier: 50 submissions/month. No backend needed.

## 4. Hosting
The site is plain HTML/CSS/JS — host anywhere:
- **Netlify** (easiest): drag the `builtvitz-site` folder onto netlify.com/drop
- **GitHub Pages**: push to a repo, enable Pages
- **Cloudflare Pages**: free, fast

You can also point a custom domain like `builtvitz.com` at any of these.
