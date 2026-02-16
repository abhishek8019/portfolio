# Portfolio Website

A modern, responsive portfolio website built with HTML, CSS, and JavaScript. This portfolio features a clean, professional design with a resume page and a projects showcase page.

## 🌟 Features

- **Responsive Design**: Fully responsive layout that works on all devices (desktop, tablet, mobile)
- **Two Main Pages**:
  - `index.html` - Resume/Home page with About, Skills, Education, and Contact sections
  - `projects.html` - Projects showcase with a grid layout
- **Dark/Light Mode**: Toggle between dark and light themes with persistent preference storage
- **Smooth Animations**: Hover effects, scroll animations, and smooth transitions
- **Mobile Menu**: Hamburger menu for mobile navigation
- **Modern Design**: Clean, professional color scheme with customizable CSS variables

## 📁 File Structure

```
/
├── index.html          # Main resume/home page
├── projects.html       # Projects showcase page
├── css/
│   └── styles.css      # All styling (responsive, animations, themes)
├── js/
│   └── main.js         # JavaScript functionality (menu, theme, animations)
└── README.md           # Documentation (this file)
```

## 🎨 Customization Guide

### 1. Personal Information

**In `index.html`:**

- **Line 14**: Update the page title
  ```html
  <title>Your Name - Professional Resume</title>
  ```

- **Line 20**: Update your name in the navigation logo
  ```html
  <div class="logo">Your Name</div>
  ```

- **Line 35**: Update the profile section
  ```html
  <h1>Your Full Name</h1>
  <p class="tagline">Software Developer | Full Stack Engineer | Tech Enthusiast</p>
  ```

- **Lines 44-54**: Customize the About Me section with your personal introduction

- **Lines 61-119**: Update your skills in each category (Frontend, Backend, Tools, Soft Skills)

- **Lines 126-147**: Update your education history

- **Lines 155-177**: Update your contact information (email, phone, location)

- **Lines 181-196**: Update social media links with your actual profiles

- **Line 204**: Update copyright year and name

**In `projects.html`:**

- **Line 6 & 20**: Update your name in the title and logo

- **Lines 36-37**: Customize the projects page heading

- **Lines 45-156**: Customize each project card:
  - Project title
  - Description
  - Technologies/tags
  - GitHub repository link
  - Live demo link
  - Change emoji in `project-image` div or replace with actual images

### 2. Adding Your Own Project Images

Replace the emoji placeholders with actual project images:

```html
<!-- Before (placeholder) -->
<div class="project-image">🚀</div>

<!-- After (with image) -->
<div class="project-image">
  <img src="path/to/your/image.jpg" alt="Project Name" style="width: 100%; height: 100%; object-fit: cover;">
</div>
```

### 3. Adding Your Profile Photo

Replace the placeholder in `index.html`:

```html
<!-- Before (placeholder) -->
<div class="profile-photo">👤</div>

<!-- After (with image) -->
<img src="path/to/your/photo.jpg" alt="Your Name" class="profile-photo">
```

### 4. Customizing Colors

All colors are defined as CSS variables in `css/styles.css` (lines 6-19). Update these values:

```css
:root {
  --primary-color: #1e3a8a;      /* Main brand color */
  --primary-dark: #1e40af;       /* Darker shade */
  --accent-color: #3b82f6;       /* Accent/highlight color */
  --text-primary: #1f2937;       /* Main text color */
  --text-secondary: #6b7280;     /* Secondary text color */
  /* ... more variables ... */
}
```

### 5. Customizing Fonts

The site uses Google Fonts (Inter). To change the font:

1. Visit [Google Fonts](https://fonts.google.com/)
2. Select your preferred font
3. Update the font link in both HTML files (line 11-13)
4. Update the CSS variable in `styles.css`:
   ```css
   --font-primary: 'YourFont', sans-serif;
   ```

### 6. Adding More Sections

To add a new section to `index.html`:

```html
<section id="your-section" class="section">
  <div class="container">
    <h2 class="section-title">Section Title</h2>
    <!-- Your content here -->
  </div>
</section>
```

Don't forget to add a navigation link:
```html
<li><a href="#your-section" class="nav-link">Section Name</a></li>
```

### 7. Adding More Projects

Copy one of the existing project cards in `projects.html` and customize it:

```html
<article class="project-card">
  <div class="project-image">🎨</div>
  <div class="project-content">
    <h3 class="project-title">Your Project Name</h3>
    <p class="project-description">Your project description...</p>
    <div class="project-tags">
      <span class="tag">Technology 1</span>
      <span class="tag">Technology 2</span>
    </div>
    <div class="project-links">
      <a href="your-github-url" class="project-link">View Code</a>
      <a href="your-demo-url" class="project-link">Live Demo</a>
    </div>
  </div>
</article>
```

## 🚀 Deployment on GitHub Pages

### Method 1: Deploy from a Branch

1. Push your code to GitHub:
   ```bash
   git add .
   git commit -m "Initial portfolio website"
   git push origin main
   ```

2. Go to your repository on GitHub
3. Click on **Settings** > **Pages**
4. Under "Source", select the branch (usually `main`) and folder (`/ (root)`)
5. Click **Save**
6. Your site will be published at `https://yourusername.github.io/repository-name/`

### Method 2: GitHub Actions (Recommended for continuous deployment)

1. Your site will automatically deploy when you push to the main branch
2. Check the Actions tab to see deployment progress
3. Access your site at `https://yourusername.github.io/repository-name/`

### Custom Domain (Optional)

1. Buy a domain name from a domain registrar
2. In your repository settings, go to **Pages**
3. Add your custom domain
4. Update your DNS settings with your domain provider:
   - Create a CNAME record pointing to `yourusername.github.io`
   - Or create A records pointing to GitHub's IP addresses

## 🛠️ Local Development

To test your portfolio locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/portfolio.git
   cd portfolio
   ```

2. Open `index.html` in your web browser:
   - Double-click the file, or
   - Use a local server (recommended):
     ```bash
     # Python 3
     python -m http.server 8000
     
     # Node.js (using npx)
     npx http-server
     ```

3. Visit `http://localhost:8000` in your browser

## 🎯 Browser Support

This portfolio works on all modern browsers:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 License

This project is open source and available for personal use. Feel free to customize it for your own portfolio!

## 🤝 Contributing

If you find any bugs or have suggestions for improvements, feel free to open an issue or submit a pull request.

## 📧 Contact

For questions or feedback, reach out via the contact information on the website.

---

**Happy coding!** 🚀