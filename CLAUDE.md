# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal academic website for Daniel P. Gross, hosted on GitHub Pages. It is a static HTML/CSS site showcasing publications, working papers, other writing, and public datasets.

## Architecture

**Static Site Structure:**
- Pure HTML/CSS with no build process or dependencies
- Each page is a standalone HTML file with shared CSS
- All pages share identical header/footer structure with navigation
- Mobile-responsive design with hamburger menu

**Key Files:**
- `index.html` - About/homepage with biography and headshot
- `publications.html` - Published research papers organized by theme
- `workingpapers.html` - Work in progress and ongoing projects
- `otherwriting.html` - Placeholder for future content
- `publicdata.html` - Links to publicly available datasets
- `style.css` - All styling (CSS variables, typography, responsive layout)
- `photo.jpg` - Headshot image

## Design System

**CSS Variables** (defined in `:root` in style.css):
- Color scheme: neutral backgrounds with accent colors for links
- Typography: Source Serif 4 for body, DM Sans for headings
- Max content width: 900px

**Consistent Components:**
- Header: Sticky navigation with site title and nav links
- Paper entries: Structured with title, authors, venue, and extra metadata (media links, data links)
- Responsive breakpoint: 700px for mobile layout

## Common Tasks

**Adding a new publication:**
1. Edit the appropriate HTML file (publications.html or workingpapers.html)
2. Follow existing paper markup structure with numbered entries
3. Include paper-title, paper-authors, paper-venue, and paper-extra divs as needed
4. Papers within each section are numbered in reverse chronological order

**Adding a new page:**
1. Copy header/footer structure from any existing page
2. Update navigation links to mark the new page as active (`class="active"`)
3. Link to `style.css` in the head
4. Include the mobile navigation toggle script in the footer

**Deployment:**
- This is a GitHub Pages site - changes pushed to the `main` branch are automatically published
- No build or compilation step required
