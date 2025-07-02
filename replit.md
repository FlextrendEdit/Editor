# Video Editor Portfolio Website

## Overview

This is a comprehensive full-stack video editor portfolio website built with React, Express, and TypeScript. The application showcases a professional video editor's work through an interactive, dark-themed interface with neon accents. It features an extensive portfolio display, advanced video showcase, pricing calculator, blog, news updates, testimonials, service offerings, and a contact form for potential clients. The site includes multiple enhanced sections designed to demonstrate professional capabilities and engage visitors.

## System Architecture

The application follows a monorepo structure with clear separation between client and server code:

**Frontend (Client)**: React SPA with TypeScript, using Vite for build tooling and development server
**Backend (Server)**: Express.js REST API with TypeScript
**Database**: PostgreSQL with Drizzle ORM for type-safe database operations
**Styling**: Tailwind CSS with shadcn/ui components for consistent UI design
**State Management**: TanStack Query for server state management
**Routing**: Wouter for lightweight client-side routing

## Key Components

### Frontend Architecture
- **Component Structure**: Modular React components organized by feature (hero, about, services, portfolio, enhanced video showcase, pricing calculator, blog, news updates, testimonials, contact)
- **UI System**: shadcn/ui component library with Radix UI primitives and Tailwind CSS
- **Theme**: Dark theme with neon color scheme (green, pink, yellow) targeting video editor aesthetic
- **Typography**: Custom font stack including Orbitron for headings, Inter for body text, and Fira Code for code elements
- **Responsive Design**: Mobile-first approach with breakpoint-based responsive layouts
- **Enhanced Features**: Advanced filtering, sorting, grid/list views, interactive pricing calculator, blog with categories, news updates with filtering

### Backend Architecture
- **API Structure**: RESTful endpoints for contact form submissions, portfolio items, and testimonials
- **Data Layer**: Drizzle ORM with PostgreSQL for persistent storage
- **Storage Pattern**: Interface-based storage abstraction with both database and in-memory implementations
- **Error Handling**: Centralized error handling with proper HTTP status codes and validation

### Database Schema
- **Users**: Basic user management with username/password authentication
- **Contact Messages**: Form submissions with comprehensive project details
- **Portfolio Items**: Video projects with metadata (title, description, category, media URLs)
- **Testimonials**: Client reviews with ratings and project type classification
- **Blog Posts**: Content management with categories, tags, and publishing features
- **Video Showcase**: Enhanced portfolio with detailed video metadata, before/after comparisons, view counts, and engagement metrics
- **Pricing Plans**: Dynamic pricing structure with features, categories, and turnaround times
- **News Updates**: Latest achievements, awards, collaborations, and technology updates with filtering capabilities

## Data Flow

1. **Contact Form**: Client fills form → validation → API submission → database storage → success response
2. **Portfolio Display**: Static data rendering with filtering capabilities by category
3. **Testimonials**: Database-driven testimonial display with star ratings
4. **Navigation**: Smooth scrolling between sections with scroll-based UI state management

## External Dependencies

### Core Framework Dependencies
- **React 18**: Frontend framework with hooks and modern patterns
- **Express.js**: Backend web framework
- **TypeScript**: Type safety across the entire stack
- **Vite**: Build tool and development server with HMR

### Database & ORM
- **Drizzle ORM**: Type-safe database toolkit
- **@neondatabase/serverless**: Serverless PostgreSQL client
- **Drizzle Kit**: Schema management and migrations

### UI & Styling
- **Tailwind CSS**: Utility-first CSS framework
- **Radix UI**: Accessible component primitives
- **Lucide React**: Modern icon library
- **Class Variance Authority**: Component variant management

### Form & Validation
- **React Hook Form**: Form state management
- **Zod**: Schema validation
- **@hookform/resolvers**: Form validation integration

### State Management
- **TanStack Query**: Server state management and caching
- **Wouter**: Lightweight routing solution

## Deployment Strategy

The application is configured for deployment on Replit with:

**Development Mode**: 
- Vite dev server for frontend with HMR
- tsx for TypeScript execution in development
- Automatic code reloading and error overlay

**Production Build**:
- Vite builds optimized frontend bundle
- esbuild compiles server code to ESM format
- Static file serving for production assets

**Environment Configuration**:
- DATABASE_URL for PostgreSQL connection
- Node.js ESM modules throughout
- Separate client and server build processes

## Changelog

Changelog:
- July 01, 2025. Initial setup of video editor portfolio website
- July 01, 2025. Added enhanced features:
  * Enhanced Video Showcase with filtering, sorting, grid/list views, and detailed video metadata
  * Interactive Pricing Calculator with real-time estimates and add-on services
  * Blog Section with categories, featured posts, and newsletter signup
  * News Updates section with achievements, awards, collaborations, and technology updates
  * Expanded navigation to include all new sections
  * Updated database schema with new tables for enhanced functionality

## User Preferences

Preferred communication style: Simple, everyday language.