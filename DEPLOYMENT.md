# GitHub Pages Deployment Guide

## 📋 Prerequisites
- GitHub account
- Git installed on your computer
- Basic knowledge of Git commands

## 🚀 Step-by-Step Deployment

### 1. Create a New Repository on GitHub
1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name your repository (e.g., `moderntech-website`)
5. Make it public (required for free GitHub Pages)
6. Don't initialize with README (we already have one)
7. Click "Create repository"

### 2. Clone and Upload Your Project

#### Option A: Using Git Command Line
```bash
# Navigate to your project folder
cd /path/to/your/project

# Initialize Git repository
git init

# Add all files
git add .

# Make your first commit
git commit -m "Initial commit: Modern Bootstrap 5 website"

# Add your GitHub repository as origin
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

#### Option B: Using GitHub Desktop
1. Download and install [GitHub Desktop](https://desktop.github.com/)
2. Click "Add an Existing Repository from your Hard Drive"
3. Select your project folder
4. Click "Publish repository" and connect to your GitHub account

#### Option C: Upload Files Directly
1. Go to your empty repository on GitHub
2. Click "uploading an existing file"
3. Drag and drop all your project files
4. Commit the changes

### 3. Enable GitHub Pages
1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

### 4. Access Your Live Website
- Your site will be available at: `https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME`
- It may take a few minutes for the site to go live
- GitHub will show you the URL in the Pages settings

## 🔧 Project Structure
```
moderntech-website/
├── index.html              # Home page (entry point)
├── about.html              # About page
├── contact.html            # Contact page
├── 404.html                # Custom 404 error page
├── css/
│   └── styles.css          # Custom CSS styles
├── js/
│   └── main.js             # JavaScript functionality
├── assets/
│   └── images/             # Image assets (if any)
├── .gitignore              # Git ignore file
├── README.md               # Project documentation
└── DEPLOYMENT.md           # This deployment guide
```

## 🌐 Custom Domain (Optional)
If you want to use a custom domain:
1. Create a file named `CNAME` in your repository root
2. Add your domain name (e.g., `www.yoursite.com`)
3. Configure your domain's DNS settings to point to GitHub Pages

## 🔄 Updating Your Site
To update your live site:
```bash
# Make your changes to the files
# Add and commit changes
git add .
git commit -m "Update: describe your changes"

# Push to GitHub
git push origin main
```

## 📱 Testing Before Deployment
- Test your site locally by opening `index.html` in a browser
- Check all pages and functionality
- Ensure all links work correctly
- Test on different screen sizes

## 🛠️ Troubleshooting

### Site Not Loading
- Check that `index.html` is in the root directory
- Ensure GitHub Pages is enabled in repository settings
- Wait a few minutes for changes to propagate

### 404 Errors
- Verify file names match exactly (case-sensitive)
- Check that all internal links use relative paths
- Ensure `404.html` exists for custom error page

### Images Not Loading
- Use relative paths (e.g., `assets/images/photo.jpg`)
- Ensure image files are committed to the repository
- Check file extensions match exactly

## 📊 Analytics (Optional)
Add Google Analytics to track visitors:
1. Create a Google Analytics account
2. Add the tracking code to all HTML pages
3. Monitor your site's performance

## 🔒 Security Notes
- Don't commit sensitive information (API keys, passwords)
- Use environment variables for sensitive data
- Keep your repository public for free GitHub Pages

## 📞 Support
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Community Forum](https://github.community/)
- [Git Documentation](https://git-scm.com/doc)

---

**Happy Deploying!** 🚀