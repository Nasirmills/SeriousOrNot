# Overview

This is a dating application called "SeriousOrNot" built with React, Express, and PostgreSQL. The app focuses on rating users based on their relationship intentions ("serious" or "not serious") and includes features like profile creation, swiping mechanics, matching, messaging, premium subscriptions, and mandatory ID verification for safety. The application features an emotional self-reflection questionnaire system with deep, meaningful questions to foster authentic connections, with answers visible only to premium members for enhanced compatibility matching.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React with TypeScript and Vite for development
- **Routing**: Wouter for client-side routing
- **State Management**: TanStack Query for server state management
- **UI Components**: Radix UI components with shadcn/ui design system
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **File Uploads**: Uppy.js for file upload handling with Google Cloud Storage integration

## Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **API Design**: RESTful API with JSON responses
- **Authentication**: Simple session-based authentication (demo implementation)
- **File Storage**: Google Cloud Storage for user photos and media
- **Payment Processing**: Stripe integration for premium subscriptions

## Database Architecture
- **Database**: PostgreSQL with Neon Database as the provider
- **ORM**: Drizzle ORM for type-safe database operations
- **Schema**: Comprehensive schema including users, questionnaires, matches, swipes, ratings, messages, playlists, playlist songs, and playlist activities
- **Migrations**: Drizzle Kit for database migrations and schema management

## Core Features
- **User Management**: Registration, authentication, profile management with photos
- **ID Verification System**: Mandatory government ID verification with face scan authentication for safety and authenticity
- **Emotional Questionnaire System**: Deep self-reflection questionnaire covering emotional boundaries, love intentions, growth mindset, and vulnerability with premium-only access to answers
- **Discovery Engine**: Swipe-based user discovery with filtering based on preferences
- **Rating System**: "Serious" vs "Not Serious" rating mechanism that builds user reputation
- **Matching System**: Mutual swipe-based matching with real-time notifications
- **Secure Messaging**: Match-restricted messaging system ensuring only mutually liked users can communicate with comprehensive validation across all messaging endpoints
- **Collaborative Playlists**: Matched users can create and manage shared music playlists with song search, manual entry, and activity tracking
- **Instagram Integration**: Users can add their Instagram usernames to profiles for enhanced social connection
- **Premium Features**: Subscription-based premium features with Stripe integration
- **Verification Badges**: Visual indicators showing verification status (verified, pending, rejected, unverified)

## Key Design Patterns
- **Component Composition**: Reusable UI components with consistent design patterns
- **Type Safety**: Full TypeScript coverage with shared types between client and server
- **Error Handling**: Comprehensive error handling with user-friendly error messages
- **Real-time Updates**: Query invalidation for real-time data updates
- **Mobile-First**: Responsive design optimized for mobile dating app experience
- **Security-First**: Mandatory identity verification with ID document upload and face scan authentication
- **Trust and Safety**: Verification status tracking with visual badges for user authenticity

# External Dependencies

## Payment Processing
- **Stripe**: Payment processing for premium subscriptions including payment elements and subscription management

## File Storage
- **Google Cloud Storage**: Object storage for user photos with ACL-based access control
- **Uppy.js**: File upload library with dashboard interface and AWS S3 compatibility

## Database Services
- **Neon Database**: Serverless PostgreSQL database provider
- **Drizzle ORM**: Type-safe database toolkit with PostgreSQL dialect

## UI and Styling
- **Radix UI**: Headless UI component library for accessibility and functionality
- **Tailwind CSS**: Utility-first CSS framework with custom design tokens
- **Lucide React**: Icon library for consistent iconography

## Development Tools
- **Vite**: Build tool and development server with HMR support
- **TanStack Query**: Data fetching and caching library for React
- **Wouter**: Lightweight routing library for React
- **Replit Integration**: Development environment integration with cartographer and error overlay plugins