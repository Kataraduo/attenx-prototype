# AttenX Deployment Guide

This document provides detailed steps for deploying the AttenX prototype to a publicly accessible website. You can choose either GitHub Pages or Netlify, both of which offer free static website hosting services.

## Method 1: Deployment using GitHub Pages

### Step 1: Create a GitHub Repository

1. Log in to your GitHub account (if you don't have one, register at [github.com](https://github.com))
2. Click the "+" icon in the top right corner and select "New repository"
3. Recommended repository name: `attenx-prototype`
4. Select Public repository
5. Click "Create repository"

### Step 2: Upload Project Files

**Using Git command line:**

```bash
# Initialize Git repository in the project directory
git init

# Add all files to staging area
git add .

# Commit changes
git commit -m "Initial commit - AttenX prototype"

# Add remote repository (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/attenx-prototype.git

# Push to GitHub
git push -u origin main
```

**Or using GitHub Desktop:**

1. Download and install [GitHub Desktop](https://desktop.github.com/)
2. Log in to your GitHub account
3. Add local repository (select the AttenX project folder)
4. Commit all changes
5. Publish repository to GitHub

### Step 3: Enable GitHub Pages

1. On the GitHub repository page, click "Settings"
2. Scroll down to the "Pages" section
3. Under "Source", select the "main" branch
4. Click "Save"
5. Wait a few minutes, your website will be available at: `https://YOUR-USERNAME.github.io/attenx-prototype/`

## Method 2: Deployment using Netlify

### Step 1: Create a Netlify Account

1. Visit [netlify.com](https://www.netlify.com/) and register for an account (you can log in with your GitHub account)

### Step 2: Deploy the Website

**Deploy from GitHub:**

1. In the Netlify dashboard, click "New site from Git"
2. Select "GitHub" as the Git provider
3. Authorize Netlify to access your GitHub account
4. Select your AttenX repository
5. Keep the default settings and click "Deploy site"

**Or upload files directly:**

1. In the Netlify dashboard, go to the "Sites" section
2. Drag and drop the entire project folder to the designated area
3. Wait for the upload and deployment to complete

### Step 3: Customize Domain Name (Optional)

1. In the site dashboard, click "Domain settings"
2. You can use the free subdomain provided by Netlify or set up a custom domain name

## Updating the Website

Regardless of which deployment method you choose, when you make changes to the prototype, simply push the updated files to your GitHub repository, and the website will update automatically.

## Notes

- Ensure all resources (images, CSS, JavaScript) use relative paths
- Check that all links work correctly
- Test the deployed website on different devices and browsers

## Help and Support

If you encounter any issues during the deployment process, please refer to:

- [GitHub Pages documentation](https://docs.github.com/en/pages)
- [Netlify documentation](https://docs.netlify.com/)