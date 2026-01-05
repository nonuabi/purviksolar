# Purvik Eco Power Solar System Website

A modern, responsive website for Purvik Eco Power Solar System, built with HTML, CSS, and JavaScript.

## Features

- Responsive design for all devices
- Contact form with EmailJS integration
- Modern UI with smooth animations
- Mobile-friendly navigation

## Setup for GitHub Pages

### 1. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under **Source**, select **GitHub Actions** (not "Deploy from a branch")
4. Save the settings

### 2. Add GitHub Secrets

To protect your EmailJS API keys, you need to add them as GitHub Secrets:

1. Go to your repository on GitHub
2. Click **Settings** → **Secrets and variables** → **Actions**
3. Click **New repository secret** and add these three secrets:

   - **Name:** `EMAILJS_PUBLIC_KEY`
     **Value:** `S6O_3fvKJunINKrQj` (your EmailJS public key)

   - **Name:** `EMAILJS_SERVICE_ID`
     **Value:** `service_ez2xff1` (your EmailJS service ID)

   - **Name:** `EMAILJS_TEMPLATE_ID`
     **Value:** `template_l5wpppk` (your EmailJS template ID)

### 3. Deploy

1. Push your code to the `main` branch
2. The GitHub Actions workflow will automatically:
   - Replace the placeholders with your actual keys
   - Deploy the site to GitHub Pages
3. Your site will be available at: `https://[your-username].github.io/[repository-name]/`

## Local Development

For local development, you can temporarily replace the placeholders in `index.html` with your actual keys, but **never commit** those changes. The placeholders (`{{EMAILJS_PUBLIC_KEY}}`, etc.) will be replaced automatically during deployment.

## Security Notes

- ✅ API keys are stored as GitHub Secrets (encrypted)
- ✅ Keys are injected only during deployment
- ✅ Keys are never exposed in the repository
- ✅ Keys are replaced server-side before the site goes live

## Contact

For questions or issues, please contact: purviksolar@gmail.com

