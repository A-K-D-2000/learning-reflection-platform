# Learning Reflection Platform

A full-stack MERN-based learning platform designed to help users manage, track, and improve their learning progress efficiently.

![image](https://github.com/user-attachments/assets/82187ce6-e1ba-4d37-a546-c3cd5e5b77b1)

## Table of Contents
- Features
- Tools and Technologies
- Dependencies
- Prerequisites
- Environment Variables
- Installation and Setup
- Database Configuration
- Project Structure
- API Endpoints
- Frontend Pages
- NPM Scripts
- Notes

## Features

### User Features
- User Signup and Login
- Secure Authentication
- Dashboard to track learning progress
- View completed and pending topics
- Add, update, and delete learning items
- User profile management

### Developer Features
- RESTful API architecture
- Protected routes (frontend and backend)
- Modular backend structure
- API integration using Axios
- Error handling and validations
- Scalable project structure

## Tools and Technologies
- Frontend: React.js
- Backend: Node.js + Express.js
- Database: MongoDB
- API Testing: Postman
- Version Control: GitHub

## Dependencies

### Backend
- express
- mongoose
- cors
- jsonwebtoken
- dotenv

### Frontend
- react
- react-router-dom
- axios

## Prerequisites
- Node.js installed
- npm installed
- MongoDB database (local or MongoDB Atlas)
- Code editor (recommended: VS Code)

## Environment Variables

Create a `.env` file inside the `/server` folder with the following variables:

```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
PORT=5000
```

> Never share or commit your `.env` file. It is already included in `.gitignore`.

## Installation and Setup

### 1. Clone the Repository
```bash
git clone https://github.com/A-K-D-2000/learning-reflection-platform.git
cd learning-reflection-platform
```

### 2. Install Dependencies

**Root:**
```bash
npm install
```

**Backend:**
```bash
cd server
npm install
```

**Frontend:**
```bash
cd ../client
npm install
```

## Database Configuration

This project uses environment variables for database configuration. After creating your `.env` file inside `/server` as described above, no further changes to the code are needed.

Make sure your MongoDB connection string follows this format:
mongodb+srv://<username>:<password>@cluster0.mongodb.net/your-db-name
## Run the Application

**Start Backend (from root folder):**
```bash
node server/server.js
```

**Start Frontend:**
```bash
cd client
npm run dev
```

## Application URLs
- Frontend: http://localhost:3000
- Backend: http://localhost:5000

## Project Structure (after installing dependencies)
```
learning-reflection-platform/
│
├── client/
│   ├── node_modules/
│   └── ...
│
├── server/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   └── server.js
│
├── .gitignore
├── node_modules/
├── package.json
└── package-lock.json
```
*Note: Dependencies are installed in both root and client folders. Run npm install in both locations.*

## API Endpoints

### Auth
- POST /api/auth/register
- POST /api/auth/login

### Learning
- GET /api/learning
- POST /api/learning
- PUT /api/learning/:id
- DELETE /api/learning/:id

### User
- GET /api/user/profile

## Frontend Pages
- / - Home / Dashboard
- /login - Login page
- /register - Signup page
- /dashboard - Learning dashboard
- /profile - User profile

## NPM Scripts

**Server:**
```bash
node server/server.js
```

**Client:**
```bash
npm run dev
```

## Notes
- node_modules folders are not included in the repository
- They will be created automatically after running npm install
- Run npm install before starting the project
- Never hardcode your MongoDB URI or JWT secret in the code — use the `.env` file

## Future Improvements
- Notifications and reminders
- Improved UI/UX
- Progress analytics
- Mobile responsiveness

## Authors
- Amita Kumari
- Anaaya Bhattacharya
- Anjali Gour
