# Blog Application

A full-stack blog application built with Spring Boot and Next.js.

## Features

- User authentication and authorization
- Create, read, update, and delete blog posts
- Comment system for blog posts
- Responsive design
- H2 database for development

## Tech Stack

### Backend
- Spring Boot 3.x
- Spring Security
- Spring Data JPA
- H2 Database
- Maven

### Frontend
- Next.js 14
- TypeScript
- Tailwind CSS
- Shadcn UI

## Prerequisites

- Java 21 or higher
- Node.js 18 or higher
- npm or pnpm

## Getting Started

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd Blog
   ```

2. Run the Spring Boot application:
   ```bash
   ./mvnw spring-boot:run
   ```
   The backend server will start on http://localhost:8080

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd blog-front
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   pnpm install
   ```

3. Run the development server:
   ```bash
   npm run dev
   # or
   pnpm dev
   ```
   The frontend will start on http://localhost:3001

## API Endpoints

### Authentication
- POST /api/v1/auth/register - Register a new user
- POST /api/v1/auth/login - Login
- GET /api/v1/auth/me - Get current user

### Posts
- GET /api/v1/posts - Get all posts
- GET /api/v1/posts/{id} - Get a specific post
- POST /api/v1/posts - Create a new post
- PUT /api/v1/posts/{id} - Update a post
- DELETE /api/v1/posts/{id} - Delete a post

### Comments
- GET /api/v1/comments/post/{postId} - Get comments for a post
- POST /api/v1/comments - Create a new comment
- DELETE /api/v1/comments/{id} - Delete a comment

## License

This project is licensed under the MIT License. 