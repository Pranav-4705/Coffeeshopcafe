# Coffee Shop Cafe Landing Page

## Overview

This is a React-based landing page for Coffee Shop Cafe, a local Texas café located in McGregor. The application is built using a modern full-stack architecture with a React frontend and Express.js backend, styled with Tailwind CSS and utilizing shadcn/ui components for a polished user interface. The website features enhanced visuals, improved animations, and all authentic business information.

## User Preferences

Preferred communication style: Simple, everyday language.

## Recent Changes (Latest Updates)

### January 13, 2025 - Major UI Enhancement Update
- **Hero Section**: Redesigned with exterior building image, enhanced gradient overlays, floating particle effects, and improved call-to-action buttons
- **About Section**: Complete redesign with award highlights, interactive stats, and image grid layout featuring both interior photos and award recognition
- **Menu Section**: Enhanced with background decorations, improved category cards with hover effects, signature dish showcase with badges, and call-to-action
- **Hours Section**: Dynamic display showing current day highlighting, emoji decorations, glassmorphism effects, and enhanced visual hierarchy
- **Gallery Section**: Masonry-style layout with all cafe images, hover effects, descriptive overlays, and customer stats
- **Contact Section**: Comprehensive redesign with customer reviews integration, enhanced contact cards, and improved map presentation
- **Animations**: Added new CSS animations including pulse-slow, shake effects, and enhanced hover transitions
- **Contact Information**: Updated with correct address (1005 W McGregor Dr, McGregor, TX 76657), phone (+1 254-840-2027), email (CoffeeShopMcGregor@gmail.com), and Facebook page
- **Directions**: Updated all "Get Directions" buttons to use Google Maps directions URL instead of simple location links
- **Customer Reviews**: Integrated three customer review links as requested
- **Facebook Integration**: Replaced all "Call Now" buttons with "Visit Facebook" links directing to https://www.facebook.com/TheCoffeeShopCafe/#
- **Font Visibility**: Enhanced text contrast and readability throughout the site with improved color schemes and font weights
- **Customer Reviews**: Rewritten with realistic customer names (Sarah Miller, Mike Johnson, Linda Rodriguez) and authentic-sounding testimonials
- **Call-to-Action Updates**: Removed all call-to-order options and replaced with Facebook page redirects as requested

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Build Tool**: Vite for development and production builds
- **Routing**: Wouter (lightweight React router)
- **Styling**: Tailwind CSS with custom coffee-themed color palette
- **UI Components**: shadcn/ui component library with Radix UI primitives
- **State Management**: TanStack Query for server state management
- **Fonts**: Google Fonts (Playfair Display, Inter, Dancing Script)

### Backend Architecture
- **Runtime**: Node.js with Express.js
- **Language**: TypeScript with ES modules
- **Database**: PostgreSQL with Drizzle ORM
- **Database Provider**: Neon Database (serverless PostgreSQL)
- **Session Management**: PostgreSQL session store with connect-pg-simple

### Development Architecture
- **Monorepo Structure**: Client, server, and shared code in single repository
- **Hot Reloading**: Vite dev server with HMR
- **Type Safety**: Shared TypeScript types between frontend and backend

## Key Components

### Landing Page Sections
1. **Header**: Fixed navigation with phone number and smooth scrolling
2. **Hero Section**: Full-screen banner with cafe images and call-to-action buttons
3. **About Section**: Story and Texas Monthly Magazine award recognition
4. **Menu Section**: Highlights of breakfast, country-style meals, and buffet options
5. **Gallery Section**: Image showcase using attached cafe photos
6. **Hours Section**: Operating hours display
7. **Contact Section**: Google Maps integration and contact information
8. **Footer**: Social links, contact info, and site credits

### UI Component System
- Comprehensive shadcn/ui component library
- Custom animations and hover effects
- Responsive design with mobile-first approach
- Coffee-themed color scheme (browns, creams, sage greens)

### Database Schema
- User management system with username/password authentication
- Prepared for future features like reservations or customer management

## Data Flow

### Static Content Flow
1. Static cafe information and images served directly
2. Google Maps integration for location services
3. External links to Google Maps for directions

### Future Dynamic Content
- User authentication system ready for implementation
- Database schema supports user registration and management
- Session management configured for user persistence

## External Dependencies

### Core Dependencies
- **@neondatabase/serverless**: Serverless PostgreSQL driver
- **drizzle-orm**: Type-safe database ORM
- **@tanstack/react-query**: Server state management
- **wouter**: Lightweight React router
- **class-variance-authority**: Utility for component variants

### UI Dependencies
- **@radix-ui/***: Comprehensive primitive UI components
- **tailwindcss**: Utility-first CSS framework
- **lucide-react**: Icon library
- **embla-carousel-react**: Carousel functionality

### Development Dependencies
- **vite**: Build tool and dev server
- **typescript**: Type checking
- **postcss**: CSS processing
- **autoprefixer**: CSS vendor prefixing

## Deployment Strategy

### Build Process
1. **Frontend Build**: Vite builds React app to `dist/public`
2. **Backend Build**: esbuild bundles server code to `dist/index.js`
3. **Database**: Drizzle handles schema migrations

### Production Configuration
- Static file serving from Express server
- Environment-based configuration
- Database connection via environment variables
- Optimized asset loading and caching

### Development Features
- **Replit Integration**: Special development banners and cartographer plugin
- **Error Handling**: Runtime error overlay for development
- **Hot Reloading**: Full-stack development with instant updates

### Asset Management
- Images stored in `attached_assets` directory
- Optimized image loading with WebP format
- Responsive image serving

The architecture supports both the current static landing page needs and future dynamic features like online reservations, customer accounts, or content management systems.