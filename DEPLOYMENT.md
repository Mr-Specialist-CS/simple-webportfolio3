# GitHub Pages Deployment Guide

## Issue Fixed

The site was not displaying styles on GitHub Pages because:
1. The Gemfile was using `jekyll` instead of `github-pages` gem
2. The baseurl needed to be set correctly for the repository name

## Changes Made

1. **Gemfile**: Updated to use `github-pages` gem (required for GitHub Pages)
2. **_config.yml**: 
   - Set `baseurl: "/webport"` (matches your repository name)
   - Set `url: "https://hajarbanu.github.io"`
   - Added `style: compressed` for SASS

## Steps to Deploy

1. **Update your local bundle:**
   ```bash
   bundle update
   ```

2. **Test locally (with baseurl):**
   ```bash
   bundle exec jekyll serve --baseurl /webport
   ```
   Or test without baseurl for local development:
   ```bash
   bundle exec jekyll serve
   ```

3. **Commit and push to GitHub:**
   ```bash
   git add .
   git commit -m "Fix GitHub Pages deployment"
   git push origin main
   ```

4. **Enable GitHub Pages:**
   - Go to your repository settings on GitHub
   - Navigate to "Pages" in the left sidebar
   - Under "Source", select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click "Save"

5. **Wait for deployment:**
   - GitHub Pages will build your site automatically
   - It may take a few minutes for the first deployment
   - Your site will be available at: `https://hajarbanu.github.io/webport`

## Troubleshooting

If styles still don't load:

1. **Check the repository name matches baseurl:**
   - Repository: `webport`
   - Baseurl: `/webport` ✅

2. **Clear browser cache** and hard refresh (Ctrl+F5)

3. **Check GitHub Pages build logs:**
   - Go to repository → Actions tab
   - Check if the build succeeded

4. **Verify CSS file exists:**
   - After deployment, visit: `https://hajarbanu.github.io/webport/assets/css/main.css`
   - It should show the compiled CSS (not 404)

## Local Development

For local development, you can temporarily set `baseurl: ""` in `_config.yml`, but remember to change it back to `"/webport"` before pushing to GitHub.

