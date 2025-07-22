# Portfolio Website - Replit Configuration

## Overview

This is a personal portfolio website for Shubham Upadhyay, a Test Automation Lead with over 10 years of experience. The website is a modern clone inspired by utkarshjain.in but customized with Shubham's professional information, experience, and skills. The application is built as a full-stack web application with a React frontend and Express.js backend, featuring responsive design, smooth animations, and a working contact form.

## User Preferences

Preferred communication style: Simple, everyday language.

## Recent Changes (January 22, 2025)

✓ Cloned utkarshjain.in website structure and design
✓ Replaced all content with Shubham Upadhyay's professional information from resume
✓ Updated skills section with accurate technical expertise (Core Java, Spring Boot, AWS, Selenium, etc.)
✓ Implemented detailed work experience from Amazon, Morgan Stanley, Zycus, and Capgemini
✓ Added proper contact information and location details
✓ Fixed React Icons import issues and storage interface for contact form
✓ Created modern, responsive portfolio with smooth animations and professional styling

## Latest Enhancements (Integrated from Personal Website)

✓ **Personal Photos**: Added actual profile photo from shubhamupadhyay.co.in 
✓ **Document Downloads**: Added both CV and Cover Letter download buttons from Google Drive
✓ **Social Media Integration**: Added real LinkedIn, GitHub, WhatsApp, Bold Profile, and Preplaced links
✓ **Enhanced Contact Section**: Added clickable phone, email, and WhatsApp connections
✓ **Projects Showcase**: Created dedicated projects section featuring key automation work
✓ **Professional Branding**: Updated all images and links to match personal website
✓ **Comprehensive Navigation**: Added projects section to main navigation menu
✓ **Multiple Download Points**: CV and Cover Letter available in hero, about, and contact sections
✓ **Interactive Location Map**: Replaced static photo with live Google Maps embed for Mahadevpura, Bengaluru
✓ **Optimized Image Strategy**: Single professional photo placement in About section with downloads
✓ **Streamlined Downloads**: Moved CV and Cover Letter downloads to About section only
✓ **Updated Professional Title**: Changed from "Test Lead & QA Engineer" to "Test Automation Lead"
✓ **Enhanced Skills**: Added Protractor alongside Cypress & Playwright, and dedicated Appium & Mobile Testing skill
✓ **Training Addition**: Added 3-month Full Stack Java Development training from Capgemini
✓ **Social Media Integration**: Added social media handles with app icons on home page above Download CV buttons
✓ **Interactive Header**: Enhanced navigation with smooth animations, dynamic active states, and modern hover effects
✓ **Mobile Optimization**: Comprehensive mobile-first responsive design with touch-friendly elements, optimized typography, and improved layouts for mobile users
✓ **Enhanced Footer**: Complete social media integration with LinkedIn, Preplaced, WhatsApp, GitHub, and Bold Profile in attractive card layout
✓ **Highlighted Scroll Button**: User-friendly gradient scroll-to-top button with animations and mobile-optimized touch targets

## Project Status

✅ **Complete and Enhanced** - Professional portfolio website with real photos and social links
✅ **Hosted Free** - Available on Replit's free tier  
✅ **All Features Working** - Contact form, animations, responsive design, social links
✅ **Authentic Content** - All personal information, photos, and links from user's actual website integrated

## Project Status

✅ **Complete and Ready** - Professional portfolio website fully functional
✅ **Hosted Free** - Available on Replit's free tier
✅ **All Features Working** - Contact form, animations, responsive design
✅ **Customized Content** - All personal information from user's resume integrated

## System Architecture

### Full-Stack Architecture
The application follows a monorepo structure with clear separation between client, server, and shared code:

- **Frontend**: React with TypeScript, using Vite as the build tool
- **Backend**: Express.js with TypeScript running on Node.js
- **Database**: PostgreSQL with Drizzle ORM (configured for Neon Database)
- **Styling**: Tailwind CSS with shadcn/ui components
- **Deployment**: Configured for production builds with static file serving

### Project Structure
```
├── client/           # React frontend application
├── server/           # Express.js backend
├── shared/           # Shared schemas and types
├── migrations/       # Database migration files
└── dist/            # Production build output
```

## Key Components

### Frontend Architecture
- **React with TypeScript**: Modern React setup using functional components and hooks
- **Vite Build Tool**: Fast development server and optimized production builds
- **Component Library**: shadcn/ui components built on Radix UI primitives
- **Styling**: Tailwind CSS with custom design system and dark mode support
- **State Management**: React Query for server state management
- **Routing**: Wouter for lightweight client-side routing
- **Animations**: Framer Motion for smooth page transitions and interactions

### Backend Architecture
- **Express.js Server**: RESTful API with middleware for logging and error handling
- **TypeScript**: Full type safety across the backend
- **Request Validation**: Zod schemas for input validation
- **Session Management**: PostgreSQL session store using connect-pg-simple
- **Development Tools**: Custom Vite integration for hot module replacement

### Database Layer
- **Drizzle ORM**: Type-safe database operations with PostgreSQL
- **Schema Definition**: Centralized schema definitions in shared directory
- **Migrations**: Automated database migrations using drizzle-kit
- **Validation**: Zod integration for runtime type checking

## Data Flow

### Contact Form Flow
1. User fills out contact form on frontend
2. Form data is validated using Zod schemas
3. POST request sent to `/api/contact` endpoint
4. Backend validates data and stores in PostgreSQL database
5. Success/error response sent back to frontend
6. Toast notification displays result to user

### Static Content Serving
1. React application builds to static files in production
2. Express server serves static files for production deployment
3. Development mode uses Vite middleware for hot reloading

## External Dependencies

### Core Dependencies
- **@neondatabase/serverless**: PostgreSQL database connection for Neon
- **drizzle-orm**: Type-safe database ORM
- **@tanstack/react-query**: Server state management
- **@radix-ui/***: Accessible UI primitives
- **tailwindcss**: Utility-first CSS framework
- **framer-motion**: Animation library
- **wouter**: Lightweight React router

### Development Dependencies
- **vite**: Build tool and development server
- **typescript**: Type checking and compilation
- **tsx**: TypeScript execution for development
- **esbuild**: Fast JavaScript bundler for production

### UI Components
- Complete shadcn/ui component library including buttons, forms, dialogs, toasts
- Radix UI primitives for accessibility and behavior
- Custom styling with Tailwind CSS variables

## Deployment Strategy

### Development Environment
- **Hot Module Replacement**: Vite provides instant updates during development
- **TypeScript Checking**: Real-time type checking across client and server
- **Database Migrations**: `npm run db:push` for schema changes
- **Logging**: Custom request logging middleware for API endpoints

### Production Build
1. **Frontend Build**: Vite builds React app to static files
2. **Backend Build**: esbuild bundles server code with external dependencies
3. **Static Serving**: Express serves built frontend files
4. **Environment Variables**: DATABASE_URL required for PostgreSQL connection

### Build Commands
- `npm run dev`: Start development server with hot reloading
- `npm run build`: Build both frontend and backend for production
- `npm run start`: Run production server
- `npm run check`: TypeScript type checking
- `npm run db:push`: Push database schema changes

### Database Configuration
- PostgreSQL database with automatic migrations
- Connection pooling through Neon serverless driver
- Session storage using PostgreSQL tables
- Schema validation with Drizzle and Zod integration

The application is designed to be easily deployable on platforms like Replit, with all necessary configuration files and scripts included for both development and production environments.