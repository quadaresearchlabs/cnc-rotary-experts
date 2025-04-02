# CNC Rotary Experts - Hugo Website

A professional website for CNC Rotary Experts, America's premier distributor of high-precision CNC rotary tables and automation solutions. Built with Hugo using the Bigspring theme.

## Setup & Development

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (v0.80.0 or newer)
- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/) (for SCSS processing)

### Local Development

1. Clone this repository
   ```bash
   git clone <repository-url>
   cd cnc-rotary-experts
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Start the development server
   ```bash
   hugo server
   ```

4. View the site at http://localhost:1313/

## Folder Structure

- `config/` - Site configuration files
- `content/` - All site content organized by language and section
- `static/` - Static assets like images and files
- `themes/` - The Bigspring theme
- `assets/` - SCSS and JS files
- `layouts/` - Custom layouts (override theme layouts)

## Content Management

### Content Management System (CMS)

This site includes Netlify CMS for easy content management. Once deployed to Netlify, you can access the admin panel at:

```
https://your-site-name.netlify.app/admin/
```

This provides a user-friendly interface for:
- Adding/editing products
- Managing services and solutions
- Updating pages like About and Contact
- Editing homepage content
- Uploading images

### Adding New Pages Manually

To create a new page without using the CMS:

```bash
hugo new content/english/[section]/[filename].md
```

Example:
```bash
hugo new content/english/products/new-product.md
```

### Content Structure

Each content file should have frontmatter at the top:

```yaml
---
title: "Page Title"
subtitle: "Optional Subtitle"
description: "SEO description"
draft: false
---
```

### Adding Images

Place images in the `static/images/` directory and reference them in markdown as:

```markdown
![Alt text](/images/your-image.jpg)
```

## Deployment

### Building for Production

To build the site for production:

```bash
hugo --minify
```

This generates the site in the `public/` directory.

### Deployment Options

#### Option 1: Netlify with CMS (Recommended)

1. Connect your Git repository to Netlify
2. Set build command: `hugo --minify`
3. Set publish directory: `public`
4. Enable Netlify Identity
   - Go to "Site Settings" > "Identity"
   - Click "Enable Identity"
   - Under "Registration" choose "Invite only"
   - Set up email templates if desired
5. Enable Git Gateway
   - Go to "Site Settings" > "Identity" > "Services" > "Git Gateway"
   - Click "Enable Git Gateway"
6. Invite Users
   - Go to the "Identity" tab in your Netlify site dashboard
   - Click "Invite users" and enter email addresses
   - Invited users will receive an email to set up their account

After deployment, you can access the CMS at `https://your-site-name.netlify.app/admin/`

#### Option 2: Web Hosting

Upload the contents of the `public/` directory to your web hosting service.

#### Option 3: GitHub Pages

1. Set up GitHub Actions using the workflow in `.github/workflows/hugo.yml`
2. Push to GitHub and the site will deploy automatically

## Customization

### Theme Configuration

Edit theme settings in `config/_default/params.toml`

### Navigation Menus

Edit menu structure in `config/_default/menus.en.toml`

### Styling

Custom CSS can be added in `assets/scss/custom.scss`

## Support & Maintenance

### Theme Updates

To update the Bigspring theme:

```bash
git submodule update --remote --merge
```

### Hugo Updates

Check Hugo version:
```bash
hugo version
```

Update Hugo following the [official documentation](https://gohugo.io/installation/).

## Contact & Support

For support with this website, contact the web development team at [your-email@example.com]. # cnc-rotary-experts
