# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is MOY E-commerce - an Astro.js landing page for a custom pattern design service targeting the fashion industry. The site is built as a static site generator with component-based architecture.

## Development Commands

- `bun dev` - Start development server (preferred package manager)
- `bun build` - Build for production
- `bun preview` - Preview production build
- `npm run dev` / `npm run build` / `npm run preview` - Alternative with npm

## Code Architecture

### Directory Structure
- `src/components/` - Reusable Astro components (Header, Hero, Features, Process, Form, Footer)
- `src/layouts/` - Layout templates (main Layout.astro wrapper)
- `src/pages/` - Route pages (index.astro contains all content)
- `src/assets/` - Static assets (SVG files)
- `public/` - Static public files and images

### Component Pattern
All components follow this structure:
1. Astro frontmatter for imports at top
2. Component logic/props
3. HTML template with semantic markup
4. Scoped `<style>` block with component-specific CSS

### Design System
The project uses CSS custom properties defined in `src/layouts/Layout.astro`:
- `--primary: #6366f1` (indigo brand)
- `--secondary: #f59e0b` (amber accent)
- `--dark: #0f172a` (slate dark)
- Other semantic color variables

### Responsive Design
Mobile-first approach with breakpoints:
- Desktop: 1200px+
- Tablet: 768px-1024px
- Mobile landscape: 480px-768px
- Mobile: 360px-480px

## Key Technical Details

- **Framework**: Astro.js v5.10.0 with TypeScript
- **Package Manager**: Bun (preferred) with bun.lock
- **Styling**: Scoped CSS with modern features (Grid, Flexbox)
- **Content**: Spanish language, fashion/textile industry focus
- **Architecture**: Single-page application with all content on index route

## Current Status

The landing page is complete and production-ready. The contact form is implemented but needs backend integration for submissions. The site generates static HTML/CSS with no JavaScript runtime by default.