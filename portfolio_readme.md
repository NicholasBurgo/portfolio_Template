# Modern Portfolio Template

A sleek, responsive, and interactive portfolio website template built with HTML, CSS, JavaScript, and Tailwind CSS. Features smooth animations, project showcases, and a modern dark theme design.

![Portfolio Preview](images/preview.png)

## ✨ Features

- **Responsive Design** - Works perfectly on desktop, tablet, and mobile devices
- **Interactive Animations** - Mouse-following cursor, animated name letters, and smooth scrolling
- **Project Showcase** - Modal-based project details with image galleries
- **Modern UI** - Dark theme with glassmorphism effects and smooth transitions
- **Easy Customization** - Simple configuration object to personalize your portfolio
- **Performance Optimized** - Fast loading with CDN resources and efficient code

## 🚀 Quick Start

1. **Download/Clone the template**
   ```bash
   git clone [your-repo-url]
   cd portfolio-template
   ```

2. **Open `index.html` in your browser** to see the template in action

3. **Customize your information** by editing the configuration object (see [Customization Guide](#-customization-guide))

4. **Add your images** to the `images/` folder

5. **Deploy** to your preferred hosting platform

## 📁 Project Structure

```
portfolio-template/
├── index.html          # Main HTML file
├── images/            # Image assets folder
│   ├── hero-bg.jpg    # Hero section background
│   ├── projects-bg.jpg # Projects section background  
│   ├── about-bg.jpg   # About section background
│   ├── profile.jpg    # Your profile photo
│   ├── project1-1.jpg # Project screenshots
│   ├── project1-2.jpg
│   └── project2-1.jpg
├── documents/         # Documents folder
│   └── your-resume.pdf # Your resume file
└── README.md         # This file
```

## 🎨 Customization Guide

### 1. Personal Information

Edit the `portfolioConfig` object in the JavaScript section of `index.html`:

```javascript
const portfolioConfig = {
  name: {
    first: "YOUR",      // Replace with your first name
    last: "NAME"        // Replace with your last name
  },
  title: "Your Title | Your Specialization", // Your professional title
  skills: ["React", "JavaScript", "Python"], // Your technical skills
  projects: [
    // Your projects array (see Projects section below)
  ]
};
```

### 2. Contact Information

Update the contact links in the header and contact section:

```html
<!-- In header section -->
<a href="https://github.com/yourusername" target="_blank">
<a href="https://www.linkedin.com/in/yourprofile/" target="_blank">
<a href="mailto:your.email@example.com">

<!-- In contact section -->
<a href="mailto:your.email@example.com">
<a href="https://www.linkedin.com/in/yourprofile" target="_blank">
<a href="https://github.com/yourusername" target="_blank">
```

### 3. About Me Section

Update your personal description and education information:

```html
<!-- Personal description -->
<p class="text-white/80 leading-relaxed mb-8">
  Write your personal description here. Talk about your passion, current role, 
  what you're studying or working on, and what drives you.
</p>

<!-- Education section -->
<span class="block font-semibold">Your Degree</span>
Your University<br>
<span class="text-sm text-white/60">Your Concentration/Major</span><br>
<span class="text-sm text-white/60">Graduation: Your Date</span>

<!-- Availability section -->
<p class="text-white/80 leading-relaxed">
  Write about your availability and what kind of work you're looking for.
</p>
```

### 4. Projects Configuration

Add your projects to the `projects` array in the configuration:

```javascript
projects: [
  {
    title: "Project Name",
    tech: ["React", "JavaScript", "CSS"], // Technologies used
    desc: "Brief description of your project",
    longDesc: `<b>Role:</b> Your role in the project<br>
      <b>Problem:</b> What problem did this project solve?<br>
      <b>Solution:</b> How did you solve it?<br>
      <b>Key Features:</b> List the main features.`,
    images: [
      "images/project1-1.jpg",  // Project screenshots
      "images/project1-2.jpg"
    ],
    links: [
      {
        type: "github",
        url: "https://github.com/yourusername/project1"
      },
      {
        type: "live",
        url: "https://yourproject.com"
      }
    ],
    status: "Completed", // or "In Progress"
    category: "Web Development" // Project category
  }
  // Add more projects...
]
```

### 5. Skills Section

Update your skills array:

```javascript
skills: [
  "React", "JavaScript", "Python", "Node.js", 
  "SQL", "Git", "Docker", "AWS"
  // Add your skills here
]
```

## 🖼️ Image Setup

### Required Images

1. **Background Images** (1920x1080 recommended):
   - `images/hero-bg.jpg` - Hero section background
   - `images/projects-bg.jpg` - Projects section background
   - `images/about-bg.jpg` - About section background

2. **Profile Photo**:
   - `images/profile.jpg` - Your professional headshot (square format recommended)

3. **Project Screenshots**:
   - `images/project1-1.jpg`, `images/project1-2.jpg`, etc.
   - Use descriptive names for your project images

4. **Documents**:
   - `documents/your-resume.pdf` - Your resume file

### Image Optimization Tips

- Use WebP format for better compression
- Optimize images for web (compress without losing quality)
- Use appropriate dimensions (backgrounds: 1920x1080, projects: 800x600)
- Consider using tools like TinyPNG or ImageOptim

## 🎯 Deployment

### GitHub Pages
1. Push your code to a GitHub repository
2. Go to Repository Settings > Pages
3. Select source branch (usually `main`)
4. Your site will be available at `https://yourusername.github.io/repository-name`

### Netlify
1. Drag and drop your project folder to [Netlify Deploy](https://app.netlify.com/drop)
2. Or connect your GitHub repository for automatic deployments

### Vercel
1. Import your project from GitHub at [Vercel](https://vercel.com)
2. Deploy with one click

## 🎨 Customization Options

### Color Scheme
The template uses a blue accent color (`#4fc3f7`). To change it:

1. **CSS Variables**: Search and replace the color values in the `<style>` section
2. **Tailwind Classes**: Update classes like `text-blue-500`, `bg-blue-700`, etc.

### Fonts
Currently uses Inter font. To change:

1. Update the Google Fonts link in the `<head>` section
2. Update the `font-family` property in the CSS

### Animations
- **Cursor Follower**: Modify the `#follower` styles and JavaScript
- **Name Animation**: Adjust the mouse interaction effects in the JavaScript
- **Scroll Animations**: Customize the `animate-bounce-slow` and other animations

## 📱 Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🔧 Technical Details

### Dependencies
- **Tailwind CSS** - Utility-first CSS framework
- **Font Awesome** - Icons
- **Google Fonts** - Typography

### JavaScript Features
- Smooth scrolling navigation
- Interactive cursor follower
- Dynamic project modal system
- Responsive image viewer
- Animated name letters
- Background parallax effects

## 🤝 Contributing

Feel free to submit issues and enhancement requests! If you'd like to contribute:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

This template is open source and available under the [MIT License](LICENSE).

## 🆘 Support

If you encounter any issues or need help customizing the template:

1. Check the [Issues](../../issues) section
2. Create a new issue with a detailed description
3. Include screenshots if applicable

## 🌟 Showcase

If you've used this template for your portfolio, we'd love to see it! Feel free to share your customized version.

---

**Happy coding!** 🚀

*Don't forget to star ⭐ this repository if you found it helpful!*