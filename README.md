# MECHA.DEV — Portfolio Site

A cyberpunk terminal-style portfolio with a built-in admin panel. No backend, no build tools, no dependencies.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The public-facing portfolio site |
| `admin.html` | Content editor (private — don't share the URL publicly) |
| `content.json` | All your site data — edit this to update content |

## Deploy to GitHub Pages (5 minutes)

1. **Create repo** named `yourusername.github.io` on GitHub
2. **Upload all 3 files** (`index.html`, `admin.html`, `content.json`) to the root
3. **Enable Pages**: repo Settings → Pages → Source: `Deploy from branch: main / (root)`
4. **Live in ~30 seconds** at `https://yourusername.github.io`

## Editing Content

### Option A — Admin Panel (recommended)
1. Open `admin.html` in your browser (locally or at `yourusername.github.io/admin.html`)
2. Edit any section using the visual forms
3. Click **💾 EXPORT JSON** to download the updated `content.json`
4. Commit & push `content.json` to GitHub → site updates automatically

### Option B — Edit JSON directly
Open `content.json` in any text editor and modify the values. The structure is self-documenting.

## Color Codes
- `""` (empty string) = Green accent
- `"a"` = Amber/orange accent  
- `"c"` = Cyan/blue accent
- `"d"` = Dim/neutral (chips only)

## Contact Form
The contact form UI is included but needs a free service for actual email delivery.
- [Formspree.io](https://formspree.io) — add `action="https://formspree.io/f/YOUR_ID"` to the form element in `index.html`
- Or use [EmailJS](https://emailjs.com) with a few lines of JS

## Customizing Colors / Theme
All colors are CSS variables at the top of `index.html` in `:root { ... }`.
Change `--green`, `--amber`, `--cyan` etc. to retheme the entire site instantly.
