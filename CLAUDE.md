# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static GitHub Pages site for Outage Labs Inc., a 501(c)(3) non-profit focused on civic technology and infrastructure monitoring. The site showcases two mobile applications (Apagón and Bokete) with a minimalist ASCII terminal aesthetic.

## Architecture

### Bilingual Structure
- Two main HTML files: `index.html` (English) and `index-es.html` (Spanish)
- Complete parallel content structure in both languages
- Language switcher at top of each page with bold current language indicator

### Design System
- ASCII terminal aesthetic with monospace fonts (Courier New)
- Black/white color scheme (#000000/#ffffff)
- Box-shadow styling (8px offset for logo, 6px for app cards)
- Bordered boxes using Unicode characters (┌─┐) for section headers
- Responsive grid layout for app cards (1 column mobile, 2 columns desktop breakpoint at 768px)

### File Structure
```
index.html       # English landing page
index-es.html    # Spanish landing page
style.css        # Shared styles for both language versions
logo.jpg         # Company logo (200x200px with 20px border radius)
```

## Development Guidelines

### Content Updates
- When updating content, always modify BOTH language versions
- Maintain visual symmetry between English and Spanish pages
- Keep ASCII box borders aligned and consistent

### Styling Conventions
- All borders: 2-3px solid black
- Box shadows: 8px for prominent elements (logo), 6px for cards, 4px mobile
- Padding: 20px standard, 15px for nested boxes
- Monospace font stack: 'Courier New', Courier, Monaco, monospace

### Meta Tags
- Include Open Graph and Twitter card metadata on both pages
- Update og:url to match page language (index.html vs index-es.html)
- Keep descriptions synchronized across languages

### Navigation
- Single navigation element with brackets styling (via :before/:after pseudo-elements)
- Language switcher uses inline styles for current page bold indicator

## No Build System
Static HTML/CSS site with no build process, dependencies, or testing framework. Deploy directly to GitHub Pages.
