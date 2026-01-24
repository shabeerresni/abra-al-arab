# Abra Al Arab - Corporate Website

A production-ready static corporate website for Abra Al Arab, an energy & commodities trading company based in Dubai, UAE.

## Project Overview

This is a static website built with vanilla HTML, CSS, and JavaScript, designed specifically for deployment on GitHub Pages. The website showcases the company's services, leadership, clients, and provides a contact form for inquiries.

## Technology Stack

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with CSS Variables, Flexbox, and Grid
- **Vanilla JavaScript** - Navigation behavior and form validation
- **No Build Tools** - All files are ready to use directly
- **No Dependencies** - Except for Google Fonts (Inter)

## Repository Structure

```
abra-al-arab.github.io/
│
├── index.html              # Home page
├── about.html              # About Us page
├── leadership.html         # Leadership page
├── services.html           # Services page
├── clients.html            # Clients page
├── associates.html         # Associates page
├── contact.html            # Contact page
│
├── assets/
│   ├── images/
│   │   └── Rayenna_oil.jpeg        # Company logo
│   ├── icons/              # Icons directory (if needed)
│   └── fonts/              # Fonts directory (if needed)
│
├── css/
│   └── style.css           # Main stylesheet
│
├── js/
│   └── main.js             # Main JavaScript file
│
└── README.md               # This file
```

## Features

- ✅ Fully responsive design (mobile, tablet, desktop)
- ✅ Sticky navigation header
- ✅ Active page highlighting
- ✅ Mobile-friendly hamburger menu
- ✅ Contact form with client-side validation
- ✅ Professional corporate design
- ✅ SEO-friendly structure
- ✅ Lighthouse-optimized

## Local Development

1. Clone or download this repository
2. Open `index.html` in a web browser
3. No build steps or server required - works directly from file system

## Deployment on GitHub Pages

### Step 1: Create GitHub Repository

1. Create a new repository on GitHub named: `abra-al-arab.github.io`
   - **Important**: The repository name must match your GitHub username/org followed by `.github.io`
   - Alternative: If using a custom domain, any repository name works, but you'll need to configure it in Settings > Pages

2. Initialize git in your local project directory:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/shabeerresni/abra-al-arab.github.io.git
   git push -u origin main
   ```

### Step 2: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** tab
3. Scroll down to **Pages** section (left sidebar)
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

### Step 3: Access Your Website

- Your website will be available at: `https://shabeerresni.github.io/abra-al-arab.github.io/`
- Note: It may take a few minutes for the site to be published initially
- GitHub Pages provides free SSL/HTTPS automatically

## Custom Domain Setup

To use a custom domain (e.g., `www.abraalarab.com`):

### Step 1: Add CNAME File

1. Create a file named `CNAME` (no extension) in the root directory
2. Add your domain name inside (e.g., `www.abraalarab.com` or `abraalarab.com`)
3. Commit and push to GitHub:
   ```bash
   echo "www.abraalarab.com" > CNAME
   git add CNAME
   git commit -m "Add custom domain"
   git push
   ```

### Step 2: Configure DNS Records

In your domain registrar's DNS settings, add the following records:

**Option A: Using CNAME (Recommended for www subdomain)**
- Type: `CNAME`
- Name: `www`
- Value: `shabeerresni.github.io`

**Option B: Using A Records (For root domain)**
- Type: `A`
- Name: `@` (or root domain)
- Value: `185.199.108.153`
- Add additional A records:
  - `185.199.109.153`
  - `185.199.110.153`
  - `185.199.111.153`

**Option C: Using ANAME/ALIAS (If supported)**
- Type: `ANAME` or `ALIAS`
- Name: `@` (root domain)
- Value: `shabeerresni.github.io`

### Step 3: Update GitHub Pages Settings

1. Go to repository Settings > Pages
2. Under "Custom domain", enter your domain (e.g., `www.abraalarab.com`)
3. Check "Enforce HTTPS" (this will be available after DNS propagates)

**Note**: DNS propagation can take 24-48 hours. You can verify with tools like `dig` or online DNS checkers.

## Important Notes

- ⚠️ **No Backend**: This is a static website. The contact form shows a success message but doesn't actually send emails. You'll need to integrate with a service like Formspree, Netlify Forms, or set up a backend API for form submissions.
- ✅ **Relative Paths**: All file paths use relative URLs (e.g., `./css/style.css`) to work correctly on GitHub Pages
- ✅ **No Build Required**: All files are production-ready and can be used directly
- ✅ **HTTPS**: GitHub Pages provides free SSL certificates automatically

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Maintenance

### Updating Content

1. Edit the relevant HTML files directly
2. Commit and push changes:
   ```bash
   git add .
   git commit -m "Update content"
   git push
   ```
3. Changes will be live on GitHub Pages within a few minutes

### Adding Pages

1. Create a new HTML file in the root directory
2. Copy the header and footer structure from existing pages
3. Update the navigation links in all pages
4. Commit and push changes

## License

© 2024 Abra Al Arab. All rights reserved.

## Contact

For website-related inquiries, please contact the development team.

---

**Built for GitHub Pages** | **Static Website** | **No Build Tools Required**

