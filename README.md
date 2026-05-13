# Mithun Miah — Portfolio Website

Premium personal portfolio website for **Mithun Miah**, a Front-End & Full Stack Developer.

## 📁 Files Included

```
dist/
├── index.html        ← Main website (upload this)
├── robots.txt        ← SEO crawler instructions
├── sitemap.xml       ← SEO sitemap
└── README.md         ← This file
```

## 🚀 Deployment

This is a **zero-dependency, production-ready static website**. No build step needed.

### Vercel / Netlify
1. Drag and drop the folder into Vercel/Netlify dashboard
2. Deploy instantly

### cPanel / Hostinger / Namecheap
1. Upload all files to `public_html/` via File Manager or FTP
2. Your site is live immediately

### GitHub Pages
1. Create a new repo, push all files
2. Enable Pages from Settings → main branch → root

---

## ✏️ Customization Guide

### 1. Update Personal Info
Open `index.html` and search for:
- `hello@mithunmiah.dev` → replace with your real email
- `github.com/mithunmiah` → your GitHub URL
- `linkedin.com/in/mithunmiah` → your LinkedIn
- `fiverr.com/mithunmiah` → your Fiverr
- `upwork.com/freelancers/mithunmiah` → your Upwork

### 2. Add Real Profile Photo
Replace the `MM` initials avatar in the hero section with:
```html
<img src="images/mithun.jpg" alt="Mithun Miah" style="width:100%;height:100%;object-fit:cover;border-radius:50%;" />
```

### 3. Add Real Projects
In the Projects section, update the 6 project cards:
- Change the emoji thumbnail to a real screenshot (use `<img>` inside `.project-thumb`)
- Update project titles, descriptions, and tags
- Replace `href="#"` with real Live Demo and GitHub links

### 4. Enable EmailJS (Real Contact Form)
1. Create an account at https://emailjs.com
2. Create a Service (Gmail, Outlook, etc.)
3. Create an Email Template with variables: `from_name`, `reply_to`, `subject`, `message`
4. Uncomment the EmailJS block at the bottom of `index.html`
5. Replace `YOUR_PUBLIC_KEY`, `YOUR_SERVICE_ID`, `YOUR_TEMPLATE_ID`
6. Add this before `</head>`:
```html
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@4/dist/email.min.js"></script>
```

### 5. Update SEO
- Replace `https://mithunmiah.dev` with your actual domain in:
  - `<link rel="canonical">`
  - `<meta property="og:url">`
  - `sitemap.xml`
- Add a real OG image at `/og-image.jpg` (1200×630px recommended)

### 6. Add Favicon
Replace the default favicon by adding a `favicon.ico` or:
```html
<link rel="icon" type="image/png" href="images/favicon.png" />
```

---

## 🎨 Color Customization

Edit these CSS variables in the `:root` block near the top of `index.html`:

```css
:root {
  --indigo: #6366f1;     /* Primary accent */
  --purple: #a855f7;     /* Secondary accent */
  --cyan: #22d3ee;       /* Highlights */
  --bg: #07090f;         /* Main background */
  --bg2: #0d1117;        /* Alternate section bg */
}
```

---

## 📊 SEO Checklist

- [x] Title tag optimized
- [x] Meta description
- [x] Open Graph tags
- [x] Twitter Card tags
- [x] Schema.org Person markup
- [x] robots.txt
- [x] sitemap.xml
- [x] Semantic HTML structure
- [x] Canonical URL (update to your domain)

---

## ⚡ Performance Notes

- No external CSS frameworks loaded (all CSS inline)
- System fonts with Google Fonts (preconnected)
- No JavaScript frameworks — pure vanilla JS
- Minimal external dependencies
- Lazy intersection-based animations

**Estimated Lighthouse Scores:**
- Performance: 95+
- Accessibility: 90+
- Best Practices: 95+
- SEO: 100

---

## 📞 Support

Built by Mithun Miah. For customization help, reach out at hello@mithunmiah.dev
