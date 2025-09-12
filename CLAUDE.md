# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-page conference website for the Internal Medicine Department's annual conference at Buriram Hospital, Thailand. The site is built with vanilla HTML, CSS, and JavaScript, using Tailwind CSS for styling and featuring a Thai language interface.

## Development Setup

This project uses pnpm as the package manager with Vite for development:

```bash
pnpm install
pnpm dev     # Start development server  
pnpm build   # Build for production
```

## Project Structure

- **index.html** - Main HTML file containing the complete single-page application
- **public/** - Static assets
  - **agenda.json** - Conference agenda data (Thai language)
  - **Logo.png** - Main conference logo
  - **brh-logo.png** - Hospital logo
  - **cover.png** - Social media cover image
  - **favicon.ico** - Site favicon
- **package.json** - pnpm configuration with Vite and Tailwind CSS dependencies

## Architecture

### Single-Page Application
The entire website is contained in `index.html` with embedded JavaScript and CSS. Key features:
- Responsive design using Tailwind CSS with custom color scheme (`brh-*` colors)
- Vanilla JavaScript for interactivity (no framework dependencies)
- Dynamic agenda loading from JSON
- Countdown timer functionality
- Scroll animations and parallax effects
- Thai language content with English technical terms

### Configuration Variables
Key configurable constants in the JavaScript section:
- `REGISTER_URL` - Registration form link (currently Google Forms)
- `EVENT_START_ISO` / `EVENT_END_ISO` - Event dates in ISO 8601 format (Bangkok timezone)
- `LOGO_SRC` - Path to conference logo

### Key JavaScript Features
- Async agenda loading from `public/agenda.json`
- Countdown timer with automatic updates
- Intersection Observer for scroll animations
- Parallax scrolling effects
- Smooth scroll navigation
- Dynamic header hide/show on scroll

## Content Management

### Agenda Updates
Edit `public/agenda.json` to modify conference schedule. Structure:
```json
{
  "6 พฤศจิกายน 2568": [
    {
      "time": "08.00 – 08.45",
      "topic": "Session title",
      "speaker": "Speaker name or '-'"
    }
  ]
}
```

### Images
- Replace logos in `public/` directory maintaining same filenames
- Optimize images for web before adding

## Styling

- Uses Tailwind CSS via CDN with custom configuration
- Custom color palette defined for hospital branding
- Thai font (Sarabun) loaded from Google Fonts
- Responsive breakpoints follow Tailwind defaults
- Custom animations defined in embedded CSS

## Deployment

Static site deployment ready - all assets are self-contained or CDN-based.