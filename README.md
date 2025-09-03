# SecondInning Cricket Platform

SecondInning is a comprehensive cricket player development and scouting platform designed to connect players, coaches, scouts, and parents in a unified ecosystem. The platform enables player performance tracking, talent discovery, and skill development through a feature-rich web application.

## Table of Contents

- [Features](#features)
- [System Architecture](#system-architecture)
- [Installation](#installation)
- [Usage Guide](#usage-guide)
- [User Roles](#user-roles)
- [Admin Panel](#admin-panel)
- [API Documentation](#api-documentation)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Features

### Core Features

- **Player Performance Tracking**: Record and visualize cricket statistics
- **Media Management**: Upload and share videos and images of cricket performances
- **Achievement System**: Track and showcase player accomplishments
- **Networking**: Connect players with coaches and scouts
- **Scouting Tools**: Advanced search and comparison tools for talent discovery
- **Parent Engagement**: Allow parents to monitor their children's progress
- **Real-time Notifications**: Instant updates for important events
- **Announcements**: System-wide communication channel

### Technical Features

- **Responsive Design**: Mobile and desktop optimized interfaces
- **Real-time Communication**: Socket-based notifications
- **Role-based Access Control**: Tailored experiences for different user types
- **Media Moderation**: Content review system for appropriate media
- **Data Visualization**: Statistical analysis and performance graphs
- **Secure Authentication**: JWT-based authentication system

## System Architecture

SecondInning follows a modern full-stack architecture:

- **Frontend**: React-based single-page application
- **Backend**: Node.js/Express RESTful API
- **Database**: MongoDB for flexible data storage
- **Real-time Layer**: Socket.IO for instant notifications
- **File Storage**: Local file system for media storage

## Installation

### Prerequisites

- Node.js (v18.0.0 or higher)
- MongoDB (v4.0 or higher)
- npm or yarn

### Setup Instructions

2. **Install server dependencies**

```bash
cd server
npm install
```

3. **Install client dependencies**

```bash
cd ../client
npm install
```

4. **Configure environment variables**

Create a `.env` file in the server directory with the following variables:

```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/secondinning
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=24d
```

5. **Start the development servers**

In the server directory:
```bash
npm start
```

In the client directory:
```bash
npm run dev
```

The client will be available at `http://localhost:5173` and the server at `http://localhost:5000`.

## Usage Guide

### Getting Started

1. **Register an account** with the appropriate role (Player, Coach, Scout, or Parent)
2. **Complete your profile** with relevant information
3. **Explore the dashboard** tailored to your role

### For Players

- **Record match statistics**: Track your performance in matches
- **Upload media**: Share videos and images of your cricket performances
- **Earn achievements**: Complete challenges to showcase your skills
- **Build network**: Connect with coaches and scouts for opportunities

### For Coaches

- **Discover talent**: Search for players based on various criteria
- **Maintain watchlist**: Keep track of promising players
- **Compare players**: Analyze performance metrics side by side
- **Provide feedback**: Offer guidance to players for improvement

### For Scouts

- **Find prospects**: Search the player database for recruitment
- **Evaluate talent**: Review player statistics and media
- **Track potential**: Monitor player development over time
- **Connect with talent**: Reach out to promising players

### For Parents

- **Link to children**: Connect parent accounts to player accounts
- **Monitor progress**: Track your child's cricket development
- **View feedback**: See coach evaluations and suggestions
- **Track matches**: Follow match participation and performance

## User Roles

### Player

The primary user role focused on skill development and showcasing talent:
- Performance tracking
- Media portfolio
- Achievement collection
- Network building

### Coach

Focused on player development and team management:
- Player evaluation
- Performance analysis
- Feedback provision
- Talent tracking

### Scout

Focused on talent discovery and recruitment:
- Player search
- Performance assessment
- Prospect tracking
- Talent outreach

### Parent

Focused on monitoring child development:
- Progress tracking
- Coach feedback review
- Match timeline monitoring
- Development support

### Admin

🔐 Admin Access Instructions
To access the Admin Panel, follow the steps below:

Open your browser and navigate to the following URL manually:
http://localhost:5173/admin/login

Enter the admin credentials:

Username: admin

Password: admin123

Click Login to enter the Admin Dashboard.

⚠️ Note: This route must be entered manually in the browser's address bar.

Platform management and oversight:
- User management
- Content moderation
- System configuration
- Security enforcement

## Admin Panel

The admin panel provides comprehensive tools for platform management:

### Dashboard
- System metrics overview
- User statistics
- Recent activities
- Quick actions

### User Management
- View and edit user accounts
- Activate/deactivate users
- Role management
- User search

### Media Moderation
- Review uploaded content
- Approve or reject media
- Content filtering
- Moderation logs

### Announcements
- Create system-wide announcements
- Schedule publication
- Target specific user groups
- Manage existing announcements

### Activity Logs
- Monitor user actions
- Track system events
- Filter by activity type
- Export logs

### System Management
- System status monitoring
- Database backup
- Performance optimization
- Maintenance mode

### Settings
- General platform settings
- Registration controls
- Media upload settings
- Notification preferences

### Security
- Password policy configuration
- Login security settings
- Session management
- Security logs

## API Documentation

The SecondInning API is organized around RESTful principles. Main endpoints include:

- `/api/auth`: Authentication and user management
- `/api/players`: Player-specific operations
- `/api/coaches`: Coach-specific operations
- `/api/scouts`: Scout-specific operations
- `/api/parents`: Parent-specific operations
- `/api/media`: Media upload and management
- `/api/stats`: Statistics recording and retrieval
- `/api/achievements`: Achievement system
- `/api/network`: Connection and networking
- `/api/admin`: Administrative operations

## Technologies Used

### Frontend
- React
- React Router
- Tailwind CSS
- Socket.IO Client
- Recharts
- Formik & Yup
- React Icons
- Axios

### Backend
- Node.js
- Express
- MongoDB & Mongoose
- Socket.IO
- JWT Authentication
- Bcrypt
- Multer

---
© 2025 SecondInning Cricket Platform. All rights reserved. 