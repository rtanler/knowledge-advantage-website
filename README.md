# Knowledge Advantage Website

This is the official website for Knowledge Advantage - Transforming Big Knowledge into Liquid Intelligence.

## Website Structure

- `index.html` - Homepage with hero section, services preview, and contact form
- `services.html` - Detailed services page with comprehensive offerings
- `styles.css` - Complete styling for the entire website

## Local Development

To view the site locally, simply open `index.html` in your web browser:

```bash
open index.html
```

Or use a local server (recommended):

```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## Deploying to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right and select "New repository"
3. Name your repository (e.g., `knowledge-advantage-website`)
4. Set it to Public
5. Do NOT initialize with README (we already have one)
6. Click "Create repository"

### Step 2: Push Your Code to GitHub

Run these commands in your terminal from this directory:

```bash
# Add all files to git
git add .

# Create your first commit
git commit -m "Initial commit: Knowledge Advantage website"

# Add your GitHub repository as remote (replace USERNAME and REPO-NAME)
git remote add origin https://github.com/USERNAME/REPO-NAME.git

# Push your code to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Click "Pages" in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Under "Branch", select `main` and `/ (root)`
6. Click "Save"

Your site will be live at: `https://USERNAME.github.io/REPO-NAME/`

### Step 4: Connect Your Custom Domain (knowledgeadvantage.net)

1. In GitHub Pages settings, under "Custom domain", enter: `www.knowledgeadvantage.net`
2. Click "Save"
3. Wait for DNS check to complete

Then update your DNS settings at your domain registrar:

**Add these DNS records:**

For **www.knowledgeadvantage.net**:
- Type: CNAME
- Name: www
- Value: USERNAME.github.io

For **knowledgeadvantage.net** (apex domain):
- Type: A
- Name: @
- Values (add all 4):
  - 185.199.108.153
  - 185.199.109.153
  - 185.199.110.153
  - 185.199.111.153

DNS propagation can take 24-48 hours, but often happens within an hour.

## Making Updates

To update your website:

1. Make changes to the HTML/CSS files locally
2. Test them by opening in your browser
3. Commit and push changes:

```bash
git add .
git commit -m "Description of your changes"
git push
```

GitHub Pages will automatically rebuild and deploy your updated site within a few minutes.

## Contact Form Setup

The contact form currently uses a `#` action. To make it functional, you have several options:

1. **Formspree** (Recommended, Free tier available)
   - Sign up at https://formspree.io
   - Get your form endpoint
   - Update the form action in `index.html`

2. **Netlify Forms** (if you switch to Netlify hosting)
   - Just add `netlify` attribute to the form

3. **EmailJS** (Client-side email service)
   - Sign up at https://www.emailjs.com
   - Add their JavaScript library

## Features

- Responsive design (mobile, tablet, desktop)
- Modern, professional aesthetic matching original design
- SEO-friendly structure
- Fast loading (static HTML/CSS)
- Easy to maintain and update

## Technologies Used

- HTML5
- CSS3 (with CSS Grid and Flexbox)
- Google Fonts (Playfair Display, Montserrat)
- Unsplash for hero image

## Need Help?

If you need to make updates and want assistance, you can use Claude Code to help modify the site programmatically.
