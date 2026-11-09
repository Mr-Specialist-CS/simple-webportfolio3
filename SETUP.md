# Quick Setup Guide

## Step 1: Update Your Information

Edit `_config.yml` and replace:
- `name`: Your actual name
- `title_text`: Your title (e.g., "A Creative Developer")
- `github_username`: Your GitHub username
- `codecademy_username`: Your Codecademy username
- `email`: Your email address
- `description`: Your personal description

## Step 2: Add Your Images

Place these images in the `assets/images/` folder:
- `profile.jpg` - Your profile photo (recommended: 400x400px or square)
- `project1.jpg` - Screenshot of Project 1
- `project2.jpg` - Screenshot of Hour of Code project (optional)

## Step 3: Customize Content

1. **About Page** (`about.markdown`):
   - Update with your background
   - Add your qualifications
   - List your activities and experience

2. **Projects Page** (`projects.markdown`):
   - Update Project 1 description
   - Update Project 2 (Hour of Code) description
   - Add any additional projects

3. **Contact Page** (`contact.markdown`):
   - Already uses your GitHub username from config
   - Add any additional contact information if needed

## Step 4: Test Locally

```bash
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000` to preview your site.

## Step 5: Deploy

1. Push to GitHub (make sure repository is **public**)
2. Enable GitHub Pages in repository settings
3. Your site will be available at `https://yourusername.github.io/hajar_web`

## Important Notes

- ✅ Make sure your GitHub repository is **public**
- ✅ Update all placeholder text
- ✅ Add your actual images
- ✅ Test responsive design on mobile devices
- ✅ Commit changes regularly to show development progress

## Color Customization

To change colors, edit `_sass/variables.scss`:
- `$accent-orange`: Primary accent (currently #ff6b35)
- `$accent-green`: Secondary accent (currently #4ecdc4)
- `$bg-primary`: Main background (currently #1a1a1a)

