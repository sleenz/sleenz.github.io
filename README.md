# Personal Portfolio Website

A modern, responsive portfolio website designed to showcase your research papers, projects, professional experience, and CV.

## Features

- **Responsive Design** - Works perfectly on desktop, tablet, and mobile devices
- **Modern UI** - Clean and professional design with smooth animations
- **Multiple Sections**:
  - Hero section with introduction
  - About section with skills
  - Projects showcase
  - Publications/Papers section
  - Professional experience timeline
  - CV download section
  - Contact form
- **Interactive Elements** - Smooth scrolling, hover effects, and animations
- **SEO Friendly** - Optimized for search engines

## Quick Start

1. **Customize your content** in `index.html`:
   - Replace "Your Name" with your actual name
   - Update your specialty and description
   - Add your social media links (GitHub, LinkedIn, Google Scholar, Email)
   - Fill in your About section
   - Add your projects with descriptions and links
   - Add your publications/papers
   - Update your experience/internships
   - Update contact information

2. **Add your media files** to the `assets` folder:
   - `profile.jpg` - Your profile photo
   - `project1.jpg`, `project2.jpg`, `project3.jpg` - Project screenshots
   - `cv.pdf` - Your CV/Resume

3. **Customize colors** (optional) in `styles.css`:
   - Edit the CSS variables at the top of the file to match your brand colors

4. **Deploy to GitHub Pages**:
   - Push your changes to GitHub
   - Go to repository Settings → Pages
   - Select your branch (usually `main` or `master`)
   - Your site will be live at `https://yourusername.github.io`

## Customization Guide

### Updating Personal Information

Open `index.html` and update the following sections:

#### 1. Hero Section (lines ~30-50)
```html
<h1 class="hero-title">Hello, I'm <span class="highlight">Your Name</span></h1>
<p class="hero-subtitle">Researcher | Developer | [Your Specialty]</p>
```

#### 2. Social Links (lines ~51-59)
Update the URLs with your actual profiles:
- GitHub
- LinkedIn
- Google Scholar
- Email

#### 3. About Section (lines ~62-95)
- Add your photo to `assets/profile.jpg`
- Update the description text
- Modify the skills tags to match your expertise

#### 4. Projects Section (lines ~98-180)
For each project, update:
- Project title
- Description
- Technologies used (tags)
- GitHub repository link
- Demo link (if available)

Add more projects by copying the `project-card` div.

#### 5. Publications Section (lines ~183-260)
For each paper, update:
- Paper title
- Authors (bold your name)
- Conference/Journal name and year
- Abstract/description
- Links to PDF, code, and citations

#### 6. Experience Section (lines ~263-330)
For each position, update:
- Date range
- Position title
- Company/Organization name
- Description and achievements
- Skills used

#### 7. Contact Section (lines ~355-395)
Update:
- Email address
- Location
- LinkedIn URL
- GitHub URL

### Adding More Content

#### Adding More Projects
Copy this structure and add to the projects grid:

```html
<div class="project-card">
    <div class="project-image">
        <img src="assets/projectN.jpg" alt="Project N">
    </div>
    <div class="project-content">
        <h3>Project Title</h3>
        <p>Description</p>
        <div class="project-tags">
            <span>Tech1</span>
            <span>Tech2</span>
        </div>
        <div class="project-links">
            <a href="link" class="btn-small"><i class="fab fa-github"></i> Code</a>
            <a href="link" class="btn-small"><i class="fas fa-external-link-alt"></i> Demo</a>
        </div>
    </div>
</div>
```

#### Adding More Publications
Copy the paper-card structure and update accordingly.

#### Adding More Experience
Copy the timeline-item structure in the experience section.

### Customizing Colors

Edit the CSS variables in `styles.css` (lines 1-15):

```css
:root {
    --primary-color: #2563eb;  /* Main brand color */
    --secondary-color: #1e40af; /* Secondary brand color */
    --accent-color: #3b82f6;   /* Accent color */
    /* ... */
}
```

### Contact Form Integration

The contact form currently shows an alert. To make it functional, you can integrate with:

1. **Formspree** - Simple form backend
2. **EmailJS** - Send emails directly from JavaScript
3. **Netlify Forms** - If hosting on Netlify
4. **GitHub Issues** - Create issues from form submissions

Instructions for integration are in the comments in `script.js`.

## File Structure

```
.
├── index.html          # Main HTML file
├── styles.css          # Styling
├── script.js           # JavaScript functionality
├── assets/             # Media files
│   ├── profile.jpg     # Your profile photo
│   ├── project1.jpg    # Project screenshots
│   ├── project2.jpg
│   ├── project3.jpg
│   └── cv.pdf          # Your CV
└── README.md           # This file
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Technologies Used

- HTML5
- CSS3 (Flexbox, Grid, Animations)
- JavaScript (ES6+)
- Font Awesome Icons

## License

Feel free to use this template for your personal portfolio. No attribution required.

## Support

If you encounter any issues or have questions, please open an issue in the repository.

---

**Happy showcasing!** 🚀
