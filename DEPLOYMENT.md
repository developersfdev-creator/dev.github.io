# Deployment Guide for AI/ML Engineer Portfolio

This guide will help you deploy your portfolio website to GitHub Pages.

## 🚀 Quick Deployment Steps

### 1. Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in to your account
2. Click the "+" icon in the top right corner and select "New repository"
3. Name your repository (e.g., `ai-ml-portfolio` or `portfolio`)
4. Make sure it's set to "Public"
5. Don't initialize with README (we already have one)
6. Click "Create repository"

### 2. Upload Your Files

#### Option A: Using GitHub Web Interface
1. On your new repository page, click "uploading an existing file"
2. Drag and drop all the portfolio files:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `README.md`
   - `LICENSE`
   - `_config.yml`
   - `.gitignore`
3. Add a commit message like "Initial portfolio upload"
4. Click "Commit changes"

#### Option B: Using Git Command Line
```bash
# Navigate to your portfolio directory
cd /path/to/your/portfolio

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial portfolio commit"

# Add your GitHub repository as remote
git remote add origin https://github.com/yourusername/your-repo-name.git

# Push to GitHub
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"
7. Wait a few minutes for deployment

### 4. Access Your Live Site

Your portfolio will be available at:
```
https://yourusername.github.io/your-repo-name
```

## 🛠️ Customization Before Deployment

### Essential Updates

1. **Personal Information** (in `index.html`):
   - Replace "Alex Chen" with your name
   - Update email address
   - Change phone number and location
   - Update social media links (GitHub, LinkedIn, etc.)

2. **Professional Experience**:
   - Update work experience in the timeline section
   - Modify job titles, companies, and descriptions
   - Adjust years of experience

3. **Projects Section**:
   - Replace example projects with your actual projects
   - Update project descriptions and technologies
   - Add real GitHub repository links
   - Include live demo links if available

4. **Skills Section**:
   - Adjust skill percentages based on your expertise
   - Add or remove technologies as needed
   - Update skill categories

5. **Contact Information**:
   - Update email address in multiple places
   - Change phone number and location
   - Update social media profiles

### Optional Customizations

1. **Colors and Branding**:
   ```css
   /* In styles.css, update these CSS variables */
   :root {
       --primary-color: #your-color;
       --secondary-color: #your-color;
       --accent-color: #your-color;
   }
   ```

2. **Profile Image**:
   - Replace the avatar placeholder with your photo
   - Update the hero section in `index.html`

3. **Favicon**:
   - Add a `favicon.ico` file to the root directory
   - Add favicon links in the `<head>` section of `index.html`

## 📱 Testing Before Deployment

### Local Testing
1. Open `index.html` in your browser
2. Test all navigation links
3. Verify responsive design on different screen sizes
4. Test contact form functionality
5. Check all animations and interactions

### Browser Compatibility
Test your portfolio in:
- Chrome
- Firefox
- Safari
- Edge

### Mobile Testing
- Use browser developer tools to test mobile views
- Test on actual mobile devices if possible

## 🔧 Troubleshooting

### Common Issues

1. **Site not loading after deployment**:
   - Wait 5-10 minutes for GitHub Pages to build
   - Check repository settings > Pages for any error messages
   - Ensure `index.html` is in the root directory

2. **CSS/JS not loading**:
   - Check file paths in `index.html`
   - Ensure all files are in the same directory
   - Verify file names match exactly (case-sensitive)

3. **Images not displaying**:
   - Check image file paths
   - Ensure images are uploaded to the repository
   - Use relative paths, not absolute paths

4. **Contact form not working**:
   - The current form is client-side only
   - For a working form, integrate with services like:
     - Formspree
     - Netlify Forms
     - EmailJS

### Performance Optimization

1. **Image Optimization**:
   - Compress images before uploading
   - Use WebP format for better compression
   - Add proper alt tags for accessibility

2. **Code Minification**:
   - Minify CSS and JavaScript for production
   - Remove unused CSS rules
   - Optimize font loading

## 🌟 Advanced Features

### Adding a Custom Domain

1. Purchase a domain from a registrar
2. In your repository settings > Pages
3. Add your custom domain
4. Update DNS settings with your registrar
5. Enable "Enforce HTTPS"

### Analytics Integration

Add Google Analytics to track visitors:
```html
<!-- Add to <head> section of index.html -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### SEO Improvements

1. Add meta descriptions
2. Include Open Graph tags for social sharing
3. Create a sitemap.xml
4. Add structured data markup

## 📞 Support

If you encounter any issues:
1. Check the GitHub Pages documentation
2. Review the repository's Issues section
3. Test locally first to isolate the problem
4. Ensure all file paths are correct and case-sensitive

## 🎉 Congratulations!

Once deployed, your professional AI/ML portfolio will be live and accessible to potential employers, clients, and collaborators worldwide. Remember to keep it updated with your latest projects and achievements!
