# montools.github.io

> Enhancing your monday.com experience with powerful tools and integrations

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen)](https://montools.github.io)
[![Jekyll](https://img.shields.io/badge/Jekyll-3.10.0-red)](https://jekyllrb.com/)
[![Bulma](https://img.shields.io/badge/Bulma-1.0.2-00d1b2)](https://bulma.io/)

## Overview

This repository hosts the official website for **montools** - a collection of productivity applications designed to enhance your monday.com workspace experience. The site showcases our apps, provides documentation, and serves as the main hub for users and potential customers.

**🌐 Live Site:** [montools.github.io](https://montools.github.io)

## Featured Applications

### 🔍 Find & Replace
Quick and accurate text search and replace functionality for monday.com Workdocs.
- Case-sensitive search options
- Preview before replace
- Seamless integration with Workdocs

### 🛠️ Text Tools for Workdocs
Comprehensive text analysis and transformation suite for content creators.
- Word, character, and sentence counting
- Case transformations (UPPERCASE, lowercase, Title Case, etc.)
- Reading time estimation
- Built-in find and replace

## Technology Stack

- **Framework:** Jekyll 3.10.0
- **CSS Framework:** Bulma 1.0.2
- **Icons:** Font Awesome
- **Fonts:** Nunito Sans
- **Hosting:** GitHub Pages

## Local Development

### Prerequisites
- Ruby (version 2.7+)
- Bundler gem

### Setup
```bash
# Clone the repository
git clone https://github.com/montools/montools.github.io.git
cd montools.github.io

# Install dependencies
bundle install

# Serve locally (with live reload)
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

The site will be available at `http://localhost:4000`

## Project Structure

```
├── _includes/          # Reusable HTML components
│   ├── head.html      # SEO meta tags, scripts, styles
│   ├── navbar.html    # Navigation header
│   ├── footer.html    # Site footer with links
│   └── breadcrumb.html # Breadcrumb navigation
├── _layouts/          # Page templates
│   ├── 0base.html     # Base template
│   ├── index.html     # Homepage template
│   └── solution.html  # App documentation template
├── assets/            # Static assets
│   ├── css/           # Custom stylesheets
│   ├── js/            # JavaScript files
│   ├── images/        # Images and icons
│   └── media/         # Videos and demos
├── solutions/         # App documentation pages
│   ├── find_and_replace/
│   └── text_tools/
├── about.md          # About page
├── privacy.md        # Privacy policy
├── sitemap.xml       # SEO sitemap
└── robots.txt        # Search engine instructions
```

## Features

### 🎨 Design
- **Dark Theme:** Professional dark color scheme with turquoise accents
- **Mobile Responsive:** Optimized for all device sizes
- **Modern UI:** Clean, intuitive interface using Bulma CSS framework

### 🔍 SEO Optimized
- Comprehensive meta tags and Open Graph support
- XML sitemap for search engines
- JSON-LD structured data
- Canonical URLs and proper heading structure

### 🚀 User Experience
- Fast loading times
- Smooth scrolling navigation
- Back-to-top functionality
- Breadcrumb navigation
- Mobile-friendly hamburger menu

### 📱 Progressive Enhancement
- Works without JavaScript
- Graceful degradation on older browsers
- Accessibility-focused markup

## Contributing

We welcome contributions to improve the site! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Commit Guidelines
- Use descriptive commit messages
- Include co-author: `Co-Authored-By: Montools <montools@proton.me>`
- Test locally before pushing

## Adding New Applications

To add a new monday.com app to the site:

1. Create a new directory in `solutions/your-app-name/`
2. Add an `index.md` file with app details, pricing, and FAQs
3. Include app screenshots in `assets/images/your-app-name/`
4. Update `_includes/section_solutions.html` to display the new app
5. Add the new URL to `sitemap.xml`

See existing app pages for reference structure.

## Privacy & Security

- **Privacy First:** Apps operate entirely within monday.com
- **No Data Collection:** We don't store or transmit user content externally
- **Transparent Policies:** Clear privacy policies for each application
- **Secure Hosting:** HTTPS enabled via GitHub Pages

## Support

- **Email:** [montools@proton.me](mailto:montools@proton.me)
- **Website:** [montools.github.io](https://montools.github.io)
- **Issues:** Use GitHub Issues for bug reports and feature requests

## License

This project is licensed under the MIT License - see the website's terms of service for details.

## Acknowledgments

- Built with [Jekyll](https://jekyllrb.com/)
- Styled with [Bulma](https://bulma.io/)
- Icons by [Font Awesome](https://fontawesome.com/)
- Hosted on [GitHub Pages](https://pages.github.com/)

---

**montools** - Making monday.com more productive, one app at a time. ⚡