# Creative Team X — Marketing Agency Website

A premium, modern single-page website for **Creative Team X**, a full-service creative marketing agency.

![Creative Team X](assets/hero.jpg)

## ✨ Features

- **Bold, cinematic hero** with custom AI-generated background image
- **Fully responsive** — beautiful on mobile, tablet, and desktop
- **Modern dark aesthetic** with violet + cyan accents
- **Portfolio section** — Currently removed (placeholder for when real case studies are ready)
- **Smooth scrolling** navigation
- **Mobile hamburger menu**
- **Working contact form** (simulated — ready to connect to real backend)
- **6 core service offerings** presented elegantly
- **Team showcase**, testimonials, and clear process
- **Zero build step** — just open `index.html` in any browser

## 🚀 Quick Start

### View the site locally

1. Open the folder `creative-team-x`
2. Double-click `index.html` (or right-click → "Open with" your browser)

That's it. No npm, no build tools, no dependencies.

### Recommended: Serve locally for best experience

```bash
# Using Python (any version)
python -m http.server 8000

# Then open http://localhost:8000
```

Or use any simple static file server:
- **Live Server** extension in VS Code
- **http-server** via npm
- **Caddy**, **serve**, etc.

## 📁 Project Structure

```
creative-team-x/
├── README.md
├── index.html          # The complete website (single file)
└── assets/
    └── hero.jpg        # Custom AI-generated hero image
```

## 🎨 Customization Guide

### Change the brand name or colors

Open `index.html` and search for these key values:

- **Logo / Name**: Lines ~55–65 (the navbar logo block)
- **Primary accent color**: `#7C3AED` (violet) — appears throughout
- **Secondary accent**: `#22D3EE` / cyan tones
- **Background**: `#0A0A0F` (near-black)

### Replace the hero image

1. Replace `assets/hero.jpg` with your own image (recommended 1920×1080 or wider)
2. Keep the filename the same or update the `src` in the hero section

### Update portfolio case studies

The portfolio is powered by a JavaScript array called `portfolioData` near the bottom of `index.html`. Each entry contains:
- `client`
- `title`
- `image`
- `category` (`brand`, `campaign`, or `digital`)
- `metrics`
- `challenge` + `solution`
- `timeline`

Edit or add to this array to update projects.

### Update services, team, or testimonials

These are hardcoded HTML sections in `index.html`. Search for the section headings (`Services`, `The Team`, etc.).

### Real contact form (now wired)

The contact form is now connected to **Formspree** (the easiest zero-backend solution for static sites).

#### Quick setup (takes ~60 seconds)

1. Go to [https://formspree.io](https://formspree.io) and create a free account
2. Create a new form → give it a name (e.g. "Creative Team X Website")
3. Copy the endpoint URL it gives you (looks like `https://formspree.io/f/abc123xy`)
4. Open `index.html` and find this line near the contact form:
   ```html
   action="https://formspree.io/f/YOUR_FORM_ID_HERE"
   ```
5. Replace `YOUR_FORM_ID_HERE` with your real form ID (the part after `/f/`)

That's it. Submissions will now arrive in your email inbox with the subject "New project inquiry — Creative Team X website".

#### Extras you can enable in Formspree
- Turn on CAPTCHA / spam protection
- Auto-reply messages to the sender
- Email notifications to multiple addresses
- Export submissions or connect to Slack / Notion

The form gracefully handles success and error states with no page reload.

**Fallback**: If you don't configure Formspree, the form will still show a friendly error message directing people to email you directly.

## 🌐 Deployment (Free & Fast)

### Netlify (recommended)
1. Drag the entire `creative-team-x` folder into [netlify.com/drop](https://app.netlify.com/drop)
2. Done — you get a live URL instantly

Or connect via Git for continuous deployment.

### Vercel
```bash
npm i -g vercel
vercel
```

### GitHub Pages
1. Push the folder to a GitHub repo
2. Go to **Settings → Pages** → Source: `main` branch + `/ (root)`
3. Enable GitHub Pages

### Other easy hosts
- Cloudflare Pages
- Render Static Sites
- Firebase Hosting
- Surge.sh (`surge`)

## 📸 Images

- **Hero image**: Custom-generated with xAI Imagine API (included)
- **Other images**: High-quality Unsplash photos + avatar placeholders (pravatar.cc)
- **Recommended replacements**: Use your own photography or generate more custom images

## 🛠 Future Enhancements (Ideas)

- Extract CSS/JS into separate files for larger projects
- Add real analytics (Plausible, PostHog, etc.)
- Integrate a real CMS (TinaCMS, Sanity, or Contentful)
- Add blog section
- Create a "Work" archive page
- Multi-language support

## 📞 Contact

This site was built for **Creative Team X**.

Ready to launch or need modifications? Edit the files directly — everything is intentionally simple and self-contained.

---

**Built with**: Tailwind CSS (CDN), vanilla JavaScript, modern HTML5, and a whole lot of taste.

---

*Creative Team X — Bold ideas. Exceptional results.*