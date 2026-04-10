# AGENTS.md - My Portfolio

## Project Overview
Static portfolio website built with vanilla HTML, CSS, and JavaScript. Single-page application with responsive design showcasing skills and projects.

## Build/Run Commands
- **View locally**: Use any live server (e.g., `python -m http.server 8000`, `npx serve`, or VS Code Live Server)
- **No build step**: Static files only (index.html, style.css, no transpilation)

## Architecture & Structure
- **index.html**: Main entry point; semantic HTML5 with navbar, hero, skills, projects, contact, footer sections
- **style.css**: Mobile-first responsive design with media queries (mobile 768px, tablet 960px breakpoints)
- **template.html**: Alternative template (not currently used)
- **Images**: PNG photos for profile and portfolio display
- **No external dependencies**: Vanilla JS only; Google Fonts (Roboto, Inter) via CDN

## Code Style Guidelines
- **HTML**: Semantic tags (header, section, footer, nav); BEM-lite for class naming (e.g., `.nav-menu`, `.project-card`)
- **CSS**: Mobile-first approach; BEM conventions; utility classes (`.container`, `.btn`, `.btn-dark`); CSS Grid/Flexbox for layout
- **JavaScript**: IIFE pattern for namespace isolation; event delegation; passive event listeners for scroll handlers; no frameworks
- **Colors**: Primary dark #1f2937, gray #6b7280, light backgrounds
- **Typography**: System fonts first, fallback to Roboto; clamp() for responsive sizing
- **Naming**: kebab-case for classes; descriptive, functional names

## Key Components
- **Navbar**: Sticky nav with mobile hamburger menu (toggle class `nav-open`)
- **Buttons**: Base `.btn` class with variants (`.btn-dark`, `.btn-small`, `.btn-submit`)
- **Grid System**: `.container` for max-width constraint; responsive grids (1fr → 2fr → 3fr columns)
- **Forms**: Contact form with standard styling (`.form-group`, `.form-input`, `.form-label`)

## Responsive Breakpoints
- **Mobile**: < 768px (single column, hidden nav menu)
- **Tablet**: 769px - 959px (2-column grids, 2-column skills)
- **Desktop**: ≥ 960px (full multi-column layouts, 3-column skills)

## Important Notes
- Smooth scroll behavior enabled globally
- SVG icons use inline paths (Font Awesome Free icons)
- Contact form is HTML/CSS only (no backend integration yet)
- JavaScript manages nav toggle and scroll shadow effects only
