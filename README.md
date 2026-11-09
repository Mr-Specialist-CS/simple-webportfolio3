# Portfolio Website

A modern, responsive portfolio website built with Jekyll, featuring a dark theme with orange and green accents.

## Features

- ✅ **Home Page** with profile photo and introduction
- ✅ **About Page** with background, qualifications, and activities
- ✅ **Projects Page** showcasing projects with images and descriptions
- ✅ **Contact Page** with social links
- ✅ **Navigation Bar** with mobile-responsive menu
- ✅ **Footer** with quick links and social icons
- ✅ **Social Icons** linking to GitHub and Codecademy profiles
- ✅ **GitHub Repository Link** in footer
- ✅ **Responsive Design** for phones, tablets, and desktops
- ✅ **Modular Code Structure** with organized SCSS files

## Setup Instructions

1. **Install Dependencies**
   ```bash
   bundle install
   ```

2. **Update Configuration**
   - Edit `_config.yml` and update:
     - `name`: Your name
     - `title_text`: Your title/role
     - `email`: Your email
     - `description`: Your description
     - `github_username`: Your GitHub username
     - `codecademy_username`: Your Codecademy username
     - `profile_image`: Path to your profile image

3. **Add Images**
   - Place your profile photo at `assets/images/profile.jpg`
   - Add project screenshots:
     - `assets/images/project1.jpg` (for Project 1)
     - `assets/images/project2.jpg` (for Hour of Code project)

4. **Update Social Links**
   - Edit `_includes/navigation.html` and `_includes/footer.html`
   - Replace `yourusername` with your actual GitHub username
   - Update Codecademy profile link
   - Update repository link in footer

5. **Customize Content**
   - Edit `about.markdown` with your background and qualifications
   - Edit `projects.markdown` with your project details
   - Update project descriptions and technologies used

6. **Run Locally**
   ```bash
   bundle exec jekyll serve
   ```
   Visit `http://localhost:4000` to view your site

7. **Build for Production**
   ```bash
   bundle exec jekyll build
   ```

## Repository Structure

```
Hajar_web/
├── _config.yml          # Site configuration
├── _includes/           # Reusable components
│   ├── navigation.html  # Navigation bar
│   └── footer.html      # Footer with social links
├── _layouts/            # Page layouts
│   ├── default.html     # Base layout
│   ├── home.html        # Home page layout
│   └── page.html        # Standard page layout
├── _sass/               # SCSS modules
│   ├── variables.scss   # Color and spacing variables
│   ├── base.scss        # Base styles
│   ├── navigation.scss  # Navigation styles
│   ├── footer.scss      # Footer styles
│   ├── hero.scss        # Hero section styles
│   ├── services.scss    # Services section styles
│   └── pages.scss       # Page content styles
├── assets/
│   ├── css/
│   │   └── main.scss    # Main stylesheet
│   └── images/          # Images directory
├── index.markdown       # Home page
├── about.markdown       # About page
├── projects.markdown    # Projects page
└── contact.markdown     # Contact page
```

## Customization

### Colors
Edit `_sass/variables.scss` to change the color scheme:
- `$accent-orange`: Primary accent color
- `$accent-green`: Secondary accent color
- `$bg-primary`: Main background color
- `$bg-secondary`: Secondary background color

### Typography
Modify font sizes and families in `_sass/variables.scss`

### Layout
Adjust spacing and container widths in `_sass/variables.scss`

## Requirements Checklist

- [x] Home page about student exists
- [x] About page about student exists
- [x] Projects page with at least Project 1 (title + description + image) exists
- [x] No major design issues
- [x] Navigation bar and footer are present
- [x] Icons leading to student's GitHub and Codecademy profiles
- [x] Link leading to the website's public GitHub repository
- [x] Responsive design works on narrow screens
- [x] Code is clean and modular (code/files/folders nicely organized)

## Notes

- Make sure your GitHub repository is **public** as required
- Add your actual profile photo and project screenshots
- Update all placeholder text with your information
- Test the responsive design on different screen sizes
- Commit your changes regularly to show development progress

## License

This portfolio template is free to use and modify for personal projects.

