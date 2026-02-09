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
