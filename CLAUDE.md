# CLAUDE.md - montools.github.io Site Documentation

## Project Overview
This is a Jekyll-based static website for **montools**, showcasing Monday.com applications and integrations. The site is hosted on GitHub Pages and serves as the main landing page and documentation hub for montools apps.

**Live Site:** https://montools.github.io  
**Repository:** https://github.com/montools/montools.github.io

## Project Structure

### Technology Stack
- **Framework:** Jekyll 3.10.0 (Ruby-based static site generator)
- **CSS Framework:** Bulma 1.0.2
- **Icons:** Font Awesome
- **Fonts:** Nunito Sans
- **Hosting:** GitHub Pages

### Core Files & Directories

#### Configuration
- `_config.yml` - Jekyll configuration (site title: "montools")
- `Gemfile` - Ruby dependencies
- `robots.txt` - Search engine crawler instructions
- `sitemap.xml` - XML sitemap for SEO

#### Layouts (`_layouts/`)
- `0base.html` - Base layout with navbar, breadcrumbs, content, back-to-top button, footer
- `index.html` - Homepage layout using greetings and solutions sections
- `index-solutions.html` - Solutions index page layout
- `solution.html` - Individual solution page layout

#### Includes (`_includes/`)
- `head.html` - HTML head with SEO meta tags, Open Graph, Twitter cards, JSON-LD schema
- `navbar.html` - Fixed top navigation with mobile burger menu
- `footer.html` - Enhanced footer with organized links and copyright
- `breadcrumb.html` - Breadcrumb navigation component
- `section_greetings.html` - Homepage hero section
- `section_solutions.html` - Solutions showcase section
- `section_contact_form.html` - Contact form (if used)
- `section_parallax-2.html` - Parallax section for solution pages
- `section_parallax-3.html` - Additional parallax section

#### Pages
- `index.html` - Homepage (uses index layout)
- `about.md` - About page with company story and mission
- `privacy.md` - Comprehensive privacy policy
- `solutions/index.md` - Solutions overview page
- `solutions/find_and_replace/index.md` - Find & Replace app documentation
- `solutions/text_tools/index.md` - Text Tools app documentation

#### Assets
- `assets/css/site.css` - Custom CSS with dark theme, mobile responsiveness
- `assets/js/site.js` - JavaScript for navbar toggle and back-to-top functionality
- `assets/images/` - Logo, app icons, screenshots
- `assets/media/` - Video demonstrations of apps

## Current Apps/Solutions

### 1. Find & Replace
- **Purpose:** Quick text search and replace in Monday.com Workdocs
- **Features:** Case-sensitive search, preview before replace
- **Pricing:** Single "Wise" plan at $4/month ($3/year)
- **Install URL:** `https://auth.monday.com/oauth2/authorize?client_id=b38790ac1d91241c92c5eab1a27c52f6&response_type=install`

### 2. Text Tools for Workdocs
- **Purpose:** Text analysis, transformation, and editing suite
- **Features:** Word/character counting, case conversion, find & replace
- **Pricing:** Freemium model (Solo free, Team $5/month, Business $8/month, Pro $13/month, Enterprise $21/month)
- **Install URL:** `https://auth.monday.com/oauth2/authorize?client_id=dab9741df949b23c6aa8c5a333098f6a&response_type=install`

## Design & Styling

### Color Scheme
- **Primary:** Dark theme with black/dark gray backgrounds
- **Accent:** Turquoise (#40e0d0) for links, highlights, and CTAs
- **Text:** White text with shadows for readability
- **Borders:** Coral, yellow, and hotpink accents for parallax sections

### Typography
- **Font Family:** Nunito Sans (400, 600, 800 weights)
- **Headings:** White with text shadows, responsive font sizes
- **Body:** White text, good contrast against dark backgrounds

### Responsive Design
- Mobile-first approach with specific breakpoints at 768px and 480px
- Collapsible columns on mobile
- Adjusted typography scaling for smaller screens
- Mobile-optimized back-to-top button positioning

## SEO & Performance

### Meta Tags Implementation
- Dynamic page titles with site name
- Meta descriptions (fallback to site description)
- Open Graph tags for social sharing
- Twitter Card markup
- Canonical URLs
- JSON-LD structured data (Organization/SoftwareApplication schema)

### Search Engine Optimization
- XML sitemap with proper priority and change frequency
- Robots.txt allowing all crawlers
- Breadcrumb navigation for better site structure
- Semantic HTML structure

## Development Commands

### Local Development
```bash
# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

### Git Workflow
- Main branch: `main`
- Commit messages should be descriptive
- Always co-author with: `Montools <montools@proton.me>`

## Key Features Implemented

### Navigation
- Fixed top navbar with mobile burger menu
- Breadcrumb navigation (hidden on homepage)
- Enhanced footer with organized sections (Quick Links, Legal, Contact)

### User Experience
- Back-to-top button with smooth scrolling
- Mobile-responsive design
- Dark theme with turquoise accents
- Video demonstrations embedded in solution pages

### Content Management
- Each solution page includes:
  - App description and features
  - Pricing tiers
  - Installation button
  - FAQ section
  - Terms of service
  - Privacy policy
  - Screenshots and videos

## Contact & Support
- **Email:** montools@proton.me
- **Website:** montools.github.io

## Privacy & Data Handling
- Apps operate entirely within Monday.com platform
- No external data storage or transmission
- Individual apps may have specific privacy policies
- GDPR/privacy compliant with transparent policies

## File Naming Conventions
- Use lowercase with underscores for directories
- Use kebab-case for URLs
- Markdown files use `.md` extension
- Images organized by app in subdirectories

## Common Tasks

### Adding a New App/Solution
1. Create new directory in `solutions/app-name/`
2. Add `index.md` with front matter including pricing, features, FAQs
3. Add app icon to `assets/images/app-name/`
4. Update `_includes/section_solutions.html` to include new app card
5. Update `sitemap.xml` with new URL
6. Test mobile responsiveness

### Updating Pricing
- Edit the `pricing:` section in the solution's `index.md`
- Ensure pricing tables render correctly on mobile

### SEO Updates
- Meta descriptions in page front matter override defaults
- Images should include alt text
- Use semantic heading structure (h1 > h2 > h3)

## Browser Compatibility
- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile browsers (iOS Safari, Chrome Mobile)
- Progressive enhancement approach