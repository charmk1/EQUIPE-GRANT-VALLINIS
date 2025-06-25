# Real Estate Consultation Website

## Overview

This is a French real estate consultation website that provides personalized consultation services for both buyers ("Acheteur") and sellers ("Vendeur"). The application is a static website with interactive forms and features, designed with a modern, professional aesthetic using a marine blue and beige color scheme.

## System Architecture

### Frontend Architecture
- **Technology**: Pure HTML, CSS, and JavaScript (no framework dependencies)
- **Styling**: Custom CSS with CSS variables for consistent theming
- **Typography**: Google Fonts integration (Playfair Display for headings, Inter for body text)
- **Maps**: Leaflet.js integration for location-based features
- **Responsive Design**: Mobile-first approach with viewport meta tags and responsive CSS

### Static Site Architecture
- **Hosting**: Python HTTP server (development/simple hosting)
- **No Backend**: Client-side only application with no server-side processing
- **Multi-page Structure**: Separate pages for buyer and seller experiences

## Key Components

### 1. Landing Pages
- **index.html**: Main buyer consultation page
- **vendeur.html**: Seller consultation page
- Both pages share similar structure but tailored content

### 2. Design System
- **Color Palette**: 
  - Marine blue (#152239) as primary
  - Beige (#f4ecd8) as secondary
  - White and off-white variants for backgrounds
- **Interactive Elements**: 
  - Ripple effects on buttons
  - Pulse animations for CTAs
  - Smooth transitions for all interactive elements

### 3. Visual Components
- Hero sections with video backgrounds
- Form interfaces for consultation requests
- Interactive buttons with advanced hover states
- Map integration capabilities (Leaflet.js ready)

### 4. User Experience Features
- Cache prevention headers for always-fresh content
- Touch-friendly interactions (tap highlight disabled)
- Smooth animations and transitions
- Responsive design for all devices

## Data Flow

### Client-Side Only
- No server-side data processing
- Form data handling would be client-side JavaScript
- Static content delivery through Python HTTP server
- No database interactions in current implementation

### User Journey
1. User lands on appropriate page (buyer/seller)
2. Interacts with consultation forms
3. Map integration for location selection
4. Form submission (currently client-side only)

## External Dependencies

### CDN Resources
- **Google Fonts**: Playfair Display and Inter font families
- **Leaflet.js**: Map functionality and styling
- **Python HTTP Server**: Static file serving

### Development Dependencies
- Node.js 20 (configured but not actively used)
- Python 3.11 for HTTP server

## Deployment Strategy

### Development Environment
- **Replit Configuration**: Dual-server setup
  - Main server on port 5000 (primary application)
  - Test server on port 5001 (testing environment)
- **Parallel Workflow**: Both servers run simultaneously

### Production Deployment
- **Static Hosting Ready**: Can be deployed to any static hosting service
- **Python Server**: Simple HTTP server for basic hosting needs
- **Port Configuration**: External port 80 for main application

### Build Process
- **No Build Step Required**: Pure HTML/CSS/JS implementation
- **Asset Management**: External CDN dependencies
- **Cache Headers**: Implemented for development workflow

## Changelog

```
Changelog:
- June 25, 2025. Initial setup
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```

## Technical Notes

### Performance Considerations
- External font loading with display=swap for better performance
- CSS animations optimized with transform properties
- Minimal JavaScript footprint
- CDN usage for external libraries

### Accessibility Features
- Semantic HTML structure
- Proper viewport configuration
- Touch-friendly interface design
- Color contrast considerations in design system

### Future Enhancements Ready
- Database integration capability (structure supports form data collection)
- Backend API integration points available
- Multi-language support architecture partially implemented
- Advanced form validation framework ready for implementation