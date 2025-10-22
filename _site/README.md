# João Capinha's Personal Website

A modern, responsive personal website built with Jekyll featuring smooth animations and easily editable content.

## 🚀 Quick Start

### Local Development
```bash
# Install dependencies
bundle install

# Build the site
bundle exec jekyll build

# Serve locally
bundle exec jekyll serve --host 0.0.0.0 --port 4000
```

The website will be available at: http://localhost:4000

## 📝 Editing Content

The website uses Jekyll data files for easy content management. All content can be edited in the `_data/` directory:

### Home Page (`_data/home.yml`)
- **Hero section**: Title and tagline
- **Intro section**: Lead paragraph
- **Highlights**: Feature cards with icons, titles, and descriptions
- **Explore section**: Navigation cards

### About Page (`_data/about.yml`)
- **Welcome section**: Title, content, and profile image

### Site Configuration (`_data/site.yml`)
- **Site title and description**
- **Navigation menu items**

### Blog Posts
- Located in `_posts/` directory
- Use standard Jekyll front matter
- Automatically styled with modern timeline design

## 🎨 Styling

- **Main CSS**: `assets/css/style.css`
- **Color scheme**: Maintains the original green theme (#0E4E45)
- **Animations**: Smooth transitions and hover effects
- **Responsive**: Mobile-first design
- **Typography**: Inter font family for modern look

## 📁 File Structure

```
├── _data/                 # Content files (easily editable)
│   ├── home.yml          # Home page content
│   ├── about.yml         # About page content
│   └── site.yml          # Site configuration
├── _layouts/             # Jekyll layouts
│   └── default.html      # Main layout template
├── _posts/               # Blog posts
├── assets/               # Static assets
│   ├── css/             # Stylesheets
│   └── images/          # Images
├── index.md             # Home page
├── about.md             # About page
└── blog.md              # Blog listing page
```

## ✨ Features

- **Dynamic Content**: Easy to edit via YAML data files
- **Modern Design**: Clean, professional appearance with animations
- **Responsive**: Works on all device sizes
- **Fast Loading**: Optimized CSS and minimal dependencies
- **SEO Friendly**: Proper meta tags and structure
- **Accessible**: Semantic HTML and proper contrast ratios

## 🔧 Customization

### Colors
Edit the CSS variables in `assets/css/style.css`:
```css
:root {
  --primary-color: #0E4E45;
  --primary-light: #156b5f;
  --primary-lighter: #9FE2D9;
  /* ... more variables */
}
```

### Content
Simply edit the YAML files in `_data/` to update any text, titles, or descriptions.

### Adding New Pages
1. Create a new `.md` file in the root directory
2. Add the page to `_data/site.yml` navigation
3. Use the `default` layout for consistency
