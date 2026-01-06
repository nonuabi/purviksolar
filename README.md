# Purvik Eco Power Solar System Website

A modern, responsive website for Purvik Eco Power Solar System, built with HTML, CSS, and JavaScript.

🌐 **Live Website:** [https://purviksolar.com](https://purviksolar.com)

## Features

- ✅ Responsive design for all devices (mobile, tablet, desktop)
- ✅ Contact form with EmailJS integration
- ✅ Modern UI with smooth animations
- ✅ Mobile-friendly navigation menu
- ✅ HTTPS enabled with custom domain
- ✅ SEO optimized with meta tags
- ✅ Secure API key management via GitHub Secrets

## Setup for GitHub Pages

### 1. GitHub Secrets Configuration

The website uses GitHub Secrets to securely store EmailJS API keys. Make sure these secrets are configured in your repository:

1. Go to **Settings** → **Secrets and variables** → **Actions**
2. Add these three secrets:
   - `EMAILJS_PUBLIC_KEY` - Your EmailJS public key
   - `EMAILJS_SERVICE_ID` - Your EmailJS service ID
   - `EMAILJS_TEMPLATE_ID` - Your EmailJS template ID

### 2. Custom Domain Setup

The website is configured for the custom domain `purviksolar.com`:

1. In GitHub repository: **Settings** → **Pages**
2. Under **Custom domain**, enter: `purviksolar.com`
3. Enable **Enforce HTTPS** (recommended)
4. Add DNS records:
   - **A Record**: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - **CNAME Record**: `www` → `your-username.github.io`

### 3. Deployment

The site automatically deploys via GitHub Actions when you push to the `main` branch. The workflow:
- Replaces EmailJS API key placeholders with secrets
- Deploys to GitHub Pages
- Works seamlessly with custom domain and HTTPS

## Local Development

For local testing, temporarily replace the placeholders in `index.html`:
- `{{EMAILJS_PUBLIC_KEY}}`
- `{{EMAILJS_SERVICE_ID}}`
- `{{EMAILJS_TEMPLATE_ID}}`

**⚠️ Important:** Never commit these changes! The placeholders will be replaced automatically during deployment.

## Security

- ✅ API keys stored as encrypted GitHub Secrets
- ✅ Keys injected only during deployment
- ✅ HTTPS enforced for secure connections
- ✅ Content Security Policy enabled

## Contact

- **Website:** [purviksolar.com](https://purviksolar.com)
- **Email:** purviksolar@gmail.com
- **Phone:** +91 8860713352
- **Address:** Shop No. 13, Ground Floor, Keshav Plaza, Sec-19 Pratap Nagar, Jaipur, Rajasthan 302033
