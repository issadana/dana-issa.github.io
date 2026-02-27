# Dana Issa - Modern Portfolio Website

A modern, responsive, and attractive portfolio website showcasing professional experience, skills, education, and projects.

## 🌟 Features

- **Responsive Design**: Fully responsive layout that works seamlessly on all devices (desktop, tablet, mobile)
- **Modern UI/UX**: Clean, professional design with smooth animations and transitions
- **Interactive Elements**:
  - Typing animation in hero section
  - Smooth scrolling navigation
  - Animated skill bars
  - Counter animations
  - Scroll reveal animations
  - Mobile-friendly navigation menu
- **Sections**:
  - Hero/Home with dynamic typing effect
  - About section with statistics
  - Skills showcase with progress bars
  - Work experience timeline
  - Education cards
  - Project portfolio grid
  - Contact form with validation
- **Accessibility**: Keyboard navigation support and ARIA labels
- **Performance**: Optimized animations and debounced scroll events

## 🚀 Getting Started

### Quick Start

1. Clone or download this repository
2. Open `index.html` in your web browser
3. Customize the content with your information

### Deployment

#### GitHub Pages

1. Create a repository named `your-username.github.io`
2. Push the files to the repository
3. Your portfolio will be live at `https://your-username.github.io`

#### Other Hosting Options

- **Netlify**: Drag and drop the folder to [Netlify](https://netlify.com)
- **Vercel**: Import the repository to [Vercel](https://vercel.com)
- **Traditional Hosting**: Upload files via FTP to any web hosting service

## 📝 Customization Guide

### Personal Information

#### Update Your Name and Title

In `index.html`, find and update:

```html
<!-- Line ~16 -->
<title>Dana Issa | Portfolio</title>

<!-- Line ~19 -->
<div class="nav-brand">
  <a href="#home">Dana Issa</a>
</div>

<!-- Line ~42 -->
<h1 class="hero-name">Dana Issa</h1>
```

In `script.js`, update the typing animation titles (line ~67):

```javascript
const titles = ['Your Title 1', 'Your Title 2', 'Your Title 3'];
```

#### Update Contact Information

In `index.html`, find the contact section (around line ~400) and update:

- Email address
- Phone number
- Location
- Social media links (LinkedIn, GitHub, Twitter, Instagram)

### Content Updates

#### About Section

Update your bio text in the About section (around line ~85 in `index.html`)

#### Skills

1. **Technical Skills**: Update skill names and percentages (around line ~115)
2. **Tools & Technologies**: Modify skill tags (around line ~145)
3. **Soft Skills**: Update the bullet list (around line ~160)

#### Experience

Update the timeline items with your work history (around line ~180)

#### Education

Modify education cards with your academic background (around line ~240)

#### Projects

Update project cards with your portfolio work (around line ~280)

### Colors and Styling

Update the color scheme in `style.css` (lines 12-20):

```css
:root {
  --primary-color: #6366f1;
  --secondary-color: #ec4899;
  --accent-color: #14b8a6;
  /* ... other colors */
}
```

### Adding Your Photo

Replace the placeholder in the About section:

```html
<!-- Find this in index.html around line 90 -->
<div class="image-placeholder">
  <i class="fas fa-user"></i>
</div>

<!-- Replace with: -->
<img src="assets/images/profile.jpg" alt="Dana Issa" />
```

Then update the CSS:

```css
/* In style.css, update .image-wrapper */
.image-wrapper img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

### Adding a Favicon

1. Create or generate a favicon (32x32 or 64x64 pixels)
2. Save it as `favicon.ico` in the root folder, or as `assets/images/favicon.png`
3. The HTML already includes the favicon link

You can generate a favicon for free at:

- [Favicon.io](https://favicon.io/)
- [RealFaviconGenerator](https://realfavicongenerator.net/)

### Adding Project Images

Replace project placeholders:

```html
<!-- Find in index.html around line 295 -->
<div class="project-placeholder">
  <i class="fas fa-laptop-code"></i>
</div>

<!-- Replace with: -->
<img src="assets/images/project-hr-system.jpg" alt="HR Management System" />
```

Add corresponding CSS:

```css
/* In style.css */
.project-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

### CV/Resume Download

Place your CV PDF in the same folder as `index.html` and name it `DanaIssa_CV_Feb2026.pdf`, or update the link in the About section:

```html
<a href="your-cv-filename.pdf" class="btn btn-primary" download></a>
```

## 🎨 Customization Tips

### Fonts

The portfolio uses:

- **Inter** for body text
- **Playfair Display** for headings

To change fonts, update the Google Fonts import in `index.html` (line ~10) and the CSS variables in `style.css`.

### Animations

Adjust animation speeds by modifying CSS custom properties:

```css
:root {
  --transition-fast: 0.2s ease;
  --transition-base: 0.3s ease;
  --transition-slow: 0.5s ease;
}
```

## 📱 Responsive Breakpoints

- **Desktop**: > 992px
- **Tablet**: 768px - 992px
- **Mobile**: < 768px
- **Small Mobile**: < 576px

## 🔧 Technologies Used

- HTML5
- CSS3 (Flexbox, Grid, CSS Variables, Animations)
- Vanilla JavaScript (ES6+)
- Font Awesome Icons
- Google Fonts

## 📄 File Structure

```
dana-issa.github.io/
├── index.html                    # Main HTML file
├── style.css                     # CSS styles and animations
├── script.js                     # JavaScript functionality
├── 404.html                      # Custom error page
├── .gitignore                    # Git ignore rules
├── README.md                     # Documentation
├── DanaIssa_CV_Feb2026.pdf       # Your CV/Resume
└── assets/                       # Static assets folder
    ├── README.md                 # Assets documentation
    └── images/                   # Image files
        ├── (add profile photo here)
        ├── (add project screenshots here)
        └── (add favicon here)
```

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 📧 Contact Form Setup

The contact form currently shows a success notification. To make it functional:

1. **Using a Backend Service**:
   - [Formspree](https://formspree.io/)
   - [EmailJS](https://www.emailjs.com/)
   - [FormSubmit](https://formsubmit.co/)

2. **Using Your Own Backend**:
   Uncomment and modify the fetch code in `script.js` (around line ~220)

## 🚀 Performance Tips

- Optimize images before uploading (use WebP format)
- Minify CSS and JavaScript for production
- Consider using a CDN for Font Awesome and Google Fonts
- Enable gzip compression on your server

## 📝 License

Feel free to use this template for your personal portfolio. Attribution is appreciated but not required.

## 🤝 Contributing

If you find any bugs or have suggestions for improvements, feel free to open an issue or submit a pull request.

---

**Built with ❤️ by Dana Issa**

Last Updated: February 2026
