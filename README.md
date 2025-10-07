# Caplog.txt Website

A clean, fast-loading Jekyll website for the Caplog.txt project - an open, plain-text format for structured personal logging.

## 🚀 Features

- **Jekyll-powered**: Built for GitHub Pages with zero dependencies
- **Mobile-first**: Responsive design that works beautifully on all devices  
- **Fast loading**: Optimized CSS and minimal JavaScript
- **Accessible**: WCAG compliant with proper semantic markup
- **SEO optimized**: Meta tags, Open Graph, and structured content
- **Easy to maintain**: Clean, well-documented code structure

## 📁 Project Structure

```
├── _layouts/
│   └── default.html          # Main page template
├── _includes/
│   ├── header.html          # Site header with navigation
│   └── footer.html          # Site footer
├── _sass/                   # SCSS source files (currently unused)
│   ├── _config.scss         # SCSS variables and configuration  
│   ├── _variables.scss      # CSS custom properties
│   ├── _base.scss          # Base styles and typography
│   ├── _utilities.scss     # Utility classes
│   ├── _buttons.scss       # Button components
│   ├── _header.scss        # Header styles
│   ├── _footer.scss        # Footer styles
│   └── _layout.scss        # Layout components
├── assets/
│   ├── css/
│   │   └── main.css        # Compiled CSS (single file)
│   └── images/
│       └── logo.png        # Project logo (placeholder)
├── index.md                # Main content page
├── _config.yml             # Jekyll configuration
└── README.md              # This file
```

## 🛠️ Development

### Prerequisites

- Ruby 2.7+ and Bundler (for local development)
- Git

### Local Development

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd caplog-txt-website
   ```

2. **Install dependencies** (optional for GitHub Pages)
   ```bash
   bundle install
   ```

3. **Serve locally**
   ```bash
   bundle exec jekyll serve
   ```
   
   Or simply open `index.html` in a browser for basic preview.

4. **Visit** `http://localhost:4000`

### GitHub Pages Deployment

This site is configured to work seamlessly with GitHub Pages:

1. Push to the `main` branch (or configure your preferred branch)
2. Enable GitHub Pages in repository settings
3. The site will be automatically built and deployed

## 🎨 Customization

### Content Updates

- **Main content**: Edit `index.md`
- **Site configuration**: Update `_config.yml`
- **Navigation**: Modify the `navigation` section in `_config.yml`

### Styling

The site uses a single CSS file (`assets/css/main.css`) for simplicity and performance. Key features:

- **CSS Custom Properties**: Easy theming via CSS variables
- **Mobile-first**: Responsive breakpoints at 768px, 1024px, 1280px
- **Design system**: Consistent spacing, typography, and color scales
- **Component-based**: Modular CSS classes for reusability

### Adding New Sections

1. Add new sections to `index.md` with unique `id` attributes
2. Update navigation in `_config.yml` if needed
3. Add corresponding anchor links for smooth scrolling

## 📋 Content Guidelines

### Writing Style
- **Clear and concise**: Focus on benefits, not features
- **User-focused**: Address the reader directly
- **Action-oriented**: Use strong verbs and clear calls-to-action
- **Scannable**: Use headers, lists, and short paragraphs

### SEO Best Practices
- Descriptive page titles and meta descriptions
- Semantic HTML structure (H1, H2, H3 hierarchy)
- Alt text for all images
- Internal linking between sections

## 🧪 Testing

### Manual Testing Checklist

- [ ] **Mobile responsiveness**: Test on various screen sizes
- [ ] **Navigation**: All anchor links work smoothly  
- [ ] **External links**: GitHub repository and CLI links open correctly
- [ ] **Performance**: Fast loading on slow connections
- [ ] **Accessibility**: Keyboard navigation and screen reader compatibility
- [ ] **Cross-browser**: Chrome, Firefox, Safari, Edge

### Performance Targets
- **First Contentful Paint**: < 1.5s
- **Largest Contentful Paint**: < 2.5s  
- **Cumulative Layout Shift**: < 0.1
- **Time to Interactive**: < 3s

## 🚀 Production Deployment

### GitHub Pages (Recommended)

1. **Repository settings**: Enable GitHub Pages on your preferred branch
2. **Custom domain** (optional): Add CNAME file with your domain
3. **HTTPS**: Automatically enabled by GitHub Pages

### Manual Deployment

The site generates static HTML/CSS/JS that can be hosted anywhere:

```bash
# Generate static site
bundle exec jekyll build

# Deploy _site/ directory to your hosting provider
```

## 📊 Analytics and Monitoring

### Adding Analytics

To add Google Analytics or similar:

1. Add tracking code to `_includes/head.html`
2. Update `_config.yml` with your tracking ID
3. Respect user privacy with appropriate consent mechanisms

### Performance Monitoring

Consider adding:
- Google PageSpeed Insights monitoring
- Real User Monitoring (RUM) for actual user experience
- Uptime monitoring for availability

## 🤝 Contributing

### Code Style

- **HTML**: Semantic markup, proper indentation
- **CSS**: BEM methodology for class naming when possible
- **JavaScript**: ES6+ syntax, progressive enhancement
- **Markdown**: Consistent formatting, descriptive headings

### Pull Request Process

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Test thoroughly across devices and browsers
5. Update documentation if needed
6. Submit a pull request with clear description

### Issues and Bug Reports

When reporting issues, please include:
- Browser and version
- Device and screen size
- Steps to reproduce
- Expected vs actual behavior
- Screenshots if applicable

## 📄 License

This website is released under the MIT License. See the [LICENSE](LICENSE) file for details.

The Caplog.txt format specification and CLI tool have their own licensing - see their respective repositories for details.

## 🔗 Related Links

- **Format Specification**: [github.com/caplogtxt/caplog.txt](https://github.com/caplogtxt/caplog.txt)
- **CLI Tool**: [github.com/caplogtxt/caplog.txt-cli](https://github.com/caplogtxt/caplog.txt-cli)
- **Jekyll Documentation**: [jekyllrb.com](https://jekyllrb.com/)
- **GitHub Pages**: [pages.github.com](https://pages.github.com/)

---

Built with ❤️ for the Caplog.txt community