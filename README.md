# Story Blog Web Application

A full-stack web application for creating and sharing stories, built with React, Node.js, and MongoDB. Features user authentication, story management, and search capabilities, deployed using Kubernetes and Argo CD for blue-green deployments.

## 🏗️ Architecture Overview

### Frontend (React)
- Single page application built with React
- JWT-based authentication
- Responsive design with styled-components
- Features:
  - User authentication (login/signup)
  - Story browsing and reading
  - Profile management
  - Story search functionality
  - Chapter navigation
  - Image upload for profiles

### Backend (Node.js)
- RESTful API built with Express.js
- MongoDB database with Mongoose ODM
- Redis caching for improved performance
- Features:
  - JWT authentication
  - Full-text search capabilities
  - File upload handling
  - Redis caching for story content
  - Database indexing for search optimization

### Deployment Architecture
- Docker Compose

  
## 🚀 Key Features

1. **User Management**
   - User registration and authentication
   - JWT-based session management
   - Profile customization with avatar upload
   - Work history tracking

2. **Story Management**
   - Multi-chapter story creation
   - Chapter navigation
   - Story summarization
   - Full-text search across stories and chapters
  
   ## 🛠️ Technical Stack

### Frontend
```json
{
  "framework": "React",
  "state-management": "Context API",
  "routing": "react-router-dom",
  "styling": "styled-components",
  "icons": "react-feather",
  "http-client": "axios"
}
```

### Backend
```json
{
  "runtime": "Node.js",
  "framework": "Express",
  "database": "MongoDB",
  "caching": "Redis",
  "authentication": "JWT",
  "file-handling": "multer"
}
```

## 🔧 Installation & Setup

### Prerequisites
- Node.js v18.17.0
- MongoDB
- Redis
- Kubernetes cluster
- Docker

### Local Development Setup

1. **Backend Setup**
```bash
cd application/backend
npm install
cp .env.example .env  # Configure environment variables
npm start
```

3. **Docker Build**

```bash
docker-compose up -d
```

## 🔐 Security Features

1. **Authentication**
   - JWT-based token authentication
   - Password hashing using bcrypt
   - Token expiration and refresh mechanisms

3. **Application Security**
   - Input validation
   - XSS protection
   - CORS configuration
   - File upload restrictions
