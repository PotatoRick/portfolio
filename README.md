# Portfolio Site

Personal consulting portfolio for infrastructure and automation services.

## Deployment

Hosted on GitHub Pages with custom domain `portfolio.theburrow.casa`.

### DNS Configuration

Add a CNAME record in Cloudflare:
- **Type:** CNAME
- **Name:** portfolio
- **Content:** potatorick.github.io
- **Proxy status:** DNS only (gray cloud) - required for GitHub Pages

### GitHub Pages Setup

1. Push this directory to a GitHub repository
2. Go to Settings > Pages
3. Source: Deploy from branch (main)
4. Custom domain: portfolio.theburrow.casa
5. Enforce HTTPS: Enabled

## Contact Form

The contact form uses [Formspree](https://formspree.io) for form handling.

1. Create a free account at formspree.io
2. Create a new form
3. Replace `YOUR_FORM_ID` in index.html with your form ID

## Customization

- **Colors:** Edit CSS variables in `:root` at top of style.css
- **Content:** Edit index.html directly
- **Pricing:** Update service prices in the services section
- **Projects:** Add/remove project cards as needed

## Local Development

Simply open `index.html` in a browser. No build step required.

```bash
# Quick preview
python3 -m http.server 8000
# Then open http://localhost:8000
```
