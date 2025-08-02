# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based personal website and blog for Jarred Robidoux, hosted on GitHub Pages. The site features a minimalist design with custom CSS styling and includes sections for writing, music, and about pages.

## Development Commands

### Local Development
```bash
# Install dependencies
bundle install

# Serve the site locally with live reload
bundle exec jekyll serve

# Build the site for production
bundle exec jekyll build
```

### File Structure
- `_config.yml` - Main Jekyll configuration
- `_layouts/` - HTML templates (default.html, post.html)
- `_posts/` - Blog posts in Markdown format (YYYY-MM-DD-title.md)
- `_sass/` - Sass stylesheets (currently minimal)
- `assets/css/style.css` - Main stylesheet with custom styling
- `_data/navigation.yml` - Navigation menu configuration
- `_includes/` - Reusable template components
- `_site/` - Generated static site (ignored in git)

## Architecture Notes

The site uses a custom design instead of the default Minima theme. The main layout (`_layouts/default.html`) creates a centered, typography-focused design with:
- Signature-style header with "JR" branding
- Simple navigation (home, writing, music, about)
- Clean post listing on the homepage
- Custom CSS with Georgia serif font and responsive design

Posts are organized by category with separate pages for different content types (writing vs general blog posts). The navigation structure is hardcoded in the default layout rather than using the `_data/navigation.yml` file.

## Content Management

- Blog posts go in `_posts/` with Jekyll naming convention
- Custom pages (about.html, writing.html, music.html) are in the root
- Images should be placed in `assets/images/`
- The site automatically generates feeds, sitemaps, and 404 pages