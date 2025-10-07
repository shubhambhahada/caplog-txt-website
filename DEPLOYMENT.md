# Quick Deployment Guide

## GitHub Pages Deployment (Recommended)

### Option 1: Direct Repository Deployment

1. **Create new repository** on GitHub (or fork existing one)
2. **Upload these files** to the repository
3. **Enable GitHub Pages**:
   - Go to repository Settings
   - Scroll to "Pages" section
   - Select source branch (usually `main`)
   - Choose root folder `/`
   - Save settings

4. **Access your site** at `https://username.github.io/repository-name`

### Option 2: GitHub Actions Deployment

Create `.github/workflows/jekyll.yml`:

```yaml
name: Deploy Jekyll site to GitHub Pages

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

permissions:
  contents: read
  pages: write
  id-token: write

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4
      
      - name: Setup Pages
        uses: actions/configure-pages@v3
      
      - name: Build with Jekyll
        uses: actions/jekyll-build-pages@v1
        with:
          source: ./
          destination: ./_site
      
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v2

  deploy:
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    runs-on: ubuntu-latest
    needs: build
    steps:
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v2
```

## Manual Deployment

### To Any Web Host

1. **Build the site locally**:
   ```bash
   bundle install
   bundle exec jekyll build
   ```

2. **Upload `_site/` folder** to your web server's document root

### To Netlify

1. **Connect repository** to Netlify
2. **Build settings**:
   - Build command: `bundle exec jekyll build`
   - Publish directory: `_site`
3. **Deploy**

### To Vercel

1. **Import repository** in Vercel dashboard
2. **Framework preset**: Jekyll
3. **Deploy**

## Custom Domain Setup

### For GitHub Pages

1. **Add CNAME file** to repository root:
   ```
   yourdomain.com
   ```

2. **Configure DNS** with your domain provider:
   ```
   Type: CNAME
   Name: www (or @)
   Value: username.github.io
   ```

3. **Enable HTTPS** in repository settings

### SSL Certificate

GitHub Pages provides free SSL certificates automatically.
For other hosts, use Let's Encrypt or your hosting provider's SSL options.

## Pre-launch Checklist

- [ ] Test all navigation links
- [ ] Verify external GitHub links work
- [ ] Check mobile responsiveness
- [ ] Validate HTML markup
- [ ] Test page loading speed
- [ ] Verify favicon displays correctly
- [ ] Check social media preview (Open Graph)
- [ ] Test code copy functionality
- [ ] Ensure accessibility compliance

## Post-deployment

1. **Submit to search engines**
2. **Monitor with Google Analytics** (if added)
3. **Set up uptime monitoring**
4. **Share on social media**

## Troubleshooting

### Common Issues

**Site not loading**: Check GitHub Pages settings and repository visibility

**Styles not applying**: Verify `main.css` path in `_config.yml` baseurl

**Links broken**: Ensure all URLs use `relative_url` or `absolute_url` filters

**Mobile issues**: Test responsiveness at various screen sizes

### Performance Optimization

- Optimize images (compress, use modern formats)
- Minify CSS and JavaScript
- Enable gzip compression
- Use a CDN for static assets
- Implement caching headers

For more help, consult the Jekyll and GitHub Pages documentation.