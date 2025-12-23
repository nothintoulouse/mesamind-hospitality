# MesaMind | Hospitality Website

Calm, ethical AI consulting for independent hospitality.

## Project Overview

This is a static website for **MesaMind | Hospitality**, a specialized consulting service focused on helping boutique hotels, inns, glamping operators, and independent stays integrate AI thoughtfully into their operations.

## Brand Guidelines

### Colors
- **Mesa Clay**: #C75C3C (accent, links)
- **Desert Sand**: #E7CBA9 (text accents, backgrounds)
- **Sage Green**: #A0B49F (primary brand, headers)
- **Sky Blue**: #A1CBE6 (minimal use, reduced for hospitality warmth)
- **Charcoal**: #333333 (body text)
- **Soft Stone**: #F2F0EB (backgrounds)

### Typography
- **Headings**: Montserrat (ExtraLight, Light, Regular, Medium, Bold)
- **Body**: Inter (Light, Medium, Extra Bold)

## File Structure

```
mesamind-hospitality/
├── index.html          # Main landing page
├── starter-kit.html    # Starter kit detail and email capture
├── styles.css          # All styling
└── README.md           # This file
```

## Deployment to GitHub Pages

### Initial Setup

1. **Initialize Git repository:**
   ```bash
   cd /Users/brayden/Documents/mesamind-hospitality
   git init
   git add .
   git commit -m "Initial commit: MesaMind | Hospitality landing page"
   ```

2. **Create GitHub repository:**
   - Go to GitHub and create a new repository called `mesamind-hospitality`
   - Do NOT initialize with README (we already have one)

3. **Connect and push:**
   ```bash
   git remote add origin https://github.com/YOUR-USERNAME/mesamind-hospitality.git
   git branch -M main
   git push -u origin main
   ```

4. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Under "Source", select branch: `main`
   - Under "Folder", select: `/ (root)`
   - Click Save
   - Site will be published at: `https://YOUR-USERNAME.github.io/mesamind-hospitality/`

### Custom Domain Setup (mesamind.toulouse.cloud)

1. **In your DNS provider (Cloudflare):**
   - Add a CNAME record:
     - Name: `mesamind`
     - Target: `YOUR-USERNAME.github.io`
     - TTL: Auto

2. **In GitHub repository settings:**
   - Go to Settings → Pages
   - Under "Custom domain", enter: `mesamind.toulouse.cloud`
   - Click Save
   - Wait for DNS check (may take a few minutes to a few hours)
   - Enable "Enforce HTTPS" once DNS is verified

3. **Add CNAME file to repository:**
   ```bash
   echo "mesamind.toulouse.cloud" > CNAME
   git add CNAME
   git commit -m "Add custom domain"
   git push
   ```

## Future Updates

To push changes:
```bash
git add .
git commit -m "Description of changes"
git push
```

Changes will be live within a few minutes of pushing.

## To-Do / Future Pages

- [ ] `services.html` - Full service offerings with pricing
- [ ] `about.html` - Background, credibility, approach
- [ ] `faq.html` - Common questions
- [ ] Email capture backend integration
- [ ] Analytics setup
- [ ] SEO optimization
- [ ] Social media meta tags

## Contact

Part of the MesaMind family of AI consulting services.

---

Built with clean HTML/CSS. No frameworks, no build process. Intentionally simple.
