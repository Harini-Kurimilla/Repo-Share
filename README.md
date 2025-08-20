# Repo Share

A MERN-based repository sharing platform with custom version control implemented from scratch.

## Overview

Repo Share is a collaborative platform that allows developers to create, manage, and share code repositories. It features a custom version control system built from the ground up, providing core functionality similar to Git while maintaining a user-friendly interface.

## Features

- **User Management**
  - User registration and authentication
  - Profile management
  - Follow other users

- **Repository Management**
  - Create public and private repositories
  - View, update, and delete repositories
  - Toggle repository visibility

- **Version Control**
  - Initialize repositories
  - Add files to staging
  - Commit changes with messages
  - Push commits to cloud storage (AWS S3)
  - Pull commits from cloud storage
  - Revert to previous commits

- **Issue Tracking**
  - Create and manage issues
  - Track issue status (open/closed)
  - Link issues to repositories

## Tech Stack

### Backend
- Node.js with Express
- MongoDB with Mongoose
- JWT Authentication
- AWS S3 for remote storage
- Socket.IO for real-time updates

### Frontend
- React with Vite
- React Router for navigation
- Primer React components
- Axios for API requests

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- AWS account (for S3 storage)

### Installation

1. Clone the repository
   ```
   git clone https://github.com/yourusername/repo-share.git
   cd repo-share
   ```

2. Install backend dependencies
   ```
   cd backend-main
   npm install
   ```

3. Install frontend dependencies
   ```
   cd ../frontend-main
   npm install
   ```

4. Set up environment variables
   Create a `.env` file in the backend-main directory with:
   ```
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET_KEY=your_jwt_secret
   S3_BUCKET=your_s3_bucket_name
   ```

5. Start the backend server
   ```
   cd backend-main
   npm start
   ```

6. Start the frontend development server
   ```
   cd frontend-main
   npm run dev
   ```

## Usage

### Command Line Interface
The application provides a CLI for version control operations:

- Initialize a repository: `node index.js init`
- Add files to staging: `node index.js add <file>`
- Commit changes: `node index.js commit <message>`
- Push to remote: `node index.js push`
- Pull from remote: `node index.js pull`
- Revert to a commit: `node index.js revert <commitID>`

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the ISC License - see the LICENSE file for details.
