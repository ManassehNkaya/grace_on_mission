# grace_on_mission
Grace on Mission - Full Stack Web Application Architecture
Architecture Overview
3-Tier Architecture:

Presentation Tier - React/Next.js Frontend
Application Tier - Node.js/Express Backend API
Data Tier - MongoDB (NoSQL) + AWS S3 Storage


Technology Stack
Frontend (Presentation Tier)

Framework: Next.js 14 (React with SSR/SSG)
Styling: Tailwind CSS
State Management: Redux Toolkit or Zustand
Video Player: Video.js or React Player
Payment UI: Stripe Elements
Authentication: NextAuth.js

Backend (Application Tier)

Runtime: Node.js
Framework: Express.js
Authentication: JWT + Passport.js
File Upload: Multer + AWS SDK
Payment Processing: Stripe API
Email Service: SendGrid or AWS SES
Video Processing: AWS MediaConvert (optional)

Database & Storage (Data Tier)

Database: MongoDB Atlas (NoSQL)
File Storage: AWS S3
CDN: AWS CloudFront (for fast media delivery)
Cache: Redis (optional, for sessions)

✅ What's Included:
Backend (Fully Implemented)

Server Setup - Express.js with all middleware configured
Authentication System - JWT-based with register, login, refresh tokens
Database Models - 6 complete MongoDB schemas:

User (with password hashing)
Sermon (with video/thumbnail URLs)
Donation (Stripe integration)
Event
Gallery
Prayer Request


File Upload Service - Complete S3 integration for videos and images
Payment Processing - Full Stripe integration:

One-time donations
Recurring donations
Webhook handling
Payment status tracking


Sermon Management - Complete CRUD operations with video upload
Security Features - Authentication, authorization, rate limiting
Error Handling - Comprehensive error middleware
Logging - Winston logger with file rotation

Infrastructure

Docker setup with docker-compose.yml
MongoDB configuration
AWS S3 integration
Stripe webhook handling
Environment configuration template

Documentation

README.md - Complete API documentation with examples
QUICK_START.md - 5-minute setup guide
PROJECT_STRUCTURE.md - Detailed architecture explanation
Setup script for automated installation

Project Structure:
grace-on-mission/
├── backend/
│   ├── src/
│   │   ├── config/           # Database, AWS, Stripe
│   │   ├── models/           # All 6 schemas
│   │   ├── controllers/      # Business logic
│   │   ├── routes/           # API endpoints
│   │   ├── middleware/       # Auth, upload, errors
│   │   ├── services/         # S3, Stripe, email
│   │   ├── utils/            # Logger, helpers
│   │   └── server.js         # Main entry point
│   ├── package.json
│   ├── Dockerfile
│   └── README.md
├── docker-compose.yml
├── QUICK_START.md
└── PROJECT_STRUCTURE.md
To Get Started:

Extract the files
Navigate to backend folder
Run setup script: ./setup.sh
Configure .env with your credentials
Start the server: npm run dev

Key Features:

- RESTful API with 7 route modules
- JWT authentication with refresh tokens
- File uploads to AWS S3
- Stripe payment processing
- MongoDB with Mongoose ODM
- Docker containerization
- Rate limiting and security
- Comprehensive error handling
- Production-ready logging
- Full API documentation

API Endpoints Available:

/api/auth/* - Authentication (register, login, profile)
/api/sermons/* - Sermon management with video upload
/api/donations/* - Payment processing with Stripe
/api/events/* - Event management (routes ready)
/api/gallery/* - Photo gallery (routes ready)
/api/prayers/* - Prayer requests (routes ready)
/api/admin/* - Admin dashboard (routes ready)
