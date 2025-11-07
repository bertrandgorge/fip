# FIP Radio Player

## Build/Lint/Test Commands
- CSS is built using: npm run build
- No linting or testing setup
- Serve locally: `python3 -m http.server` or any static file server

## Architecture
- **Frontend**: Single HTML file with embedded CSS/JS
- **Backend**: PHP redirect to GitHub Pages
- **APIs**: Radio France GraphQL API for song metadata
- **Libraries**: jQuery, HLS.js for streaming, Google Cast SDK
- **Progressive Web App**: Service worker manifest for offline/installation

## Code Style Guidelines
- **JavaScript**: Mix of jQuery and vanilla JS, functional style
- **CSS**: Embedded in HTML head, responsive design with dark mode
- **Naming**: camelCase for variables/functions, kebab-case for CSS classes
- **Error handling**: Basic try/catch, AJAX fail handlers
- **Imports**: CDN links for external libraries (jQuery, HLS.js, Cast SDK)
