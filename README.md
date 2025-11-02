##Swift-Talk - Real-Time Chat Application
https://img.shields.io/badge/Swift--Talk-Real%2520Time%2520Chat-blue
https://img.shields.io/badge/React-18.0+-61DAFB?logo=react
https://img.shields.io/badge/Node.js-Express-green?logo=node.js

##Overview
A full-stack real-time chat application supporting one-to-one and group messaging with instant message delivery using WebSockets.

##Features
-Real-time Messaging: Instant message delivery using Socket.io WebSockets
-One-to-One & Group Chats: Support for both private and group conversations
-JWT Authentication: Secure user authentication and authorization
-Typing Indicators: Real-time typing status notifications
-Responsive Design: Mobile-friendly interface built with React and Tailwind CSS
-Message Persistence: Secure data storage using MongoDB Atlas
-High Availability: Deployed on Vercel for optimal performance

##Tech Stack
#Frontend
-ReactJS - Modern UI framework
-Tailwind CSS - Utility-first CSS framework
-Socket.io Client - Real-time communication

#Backend
-Node.js - Runtime environment
-Express.js - Web application framework
-Socket.io - WebSocket implementation
-JWT - JSON Web Tokens for authentication
-MongoDB - NoSQL database
-MongoDB Atlas - Cloud database service

#Deployment
-Vercel - Frontend and backend hosting
-GitHub - Version control

##Installation
#Prerequisites
-Node.js (v16 or higher)
-MongoDB Atlas account or local MongoDB instance

#Local Development
-Clone the repository

```bash
git clone https://github.com/FalguniJain/SwiftTalk
cd swift-talk
Install dependencies
```
bash
# Install backend dependencies
cd backend
npm install

# Install frontend dependencies  
cd ../frontend
npm install
Environment Configuration
Create a .env file in the backend directory:

env
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
PORT=5000
Run the application

bash
# Start backend server
cd backend
npm run dev

# Start frontend development server
cd ../frontend
npm run dev
Access the application
Open http://localhost:3000 in your browser

#Usage
-Register/Login: Create an account or login with existing credentials
-Start Chatting: Search for users and start one-on-one conversations
-Create Groups: Form group chats with multiple users
-Real-time Features: Enjoy instant messaging with typing indicators

##API Endpoints
#Authentication
-POST /api/auth/register - User registration
-POST /api/auth/login - User login
-GET /api/auth/verify - Verify JWT token

#Users
-GET /api/users - Get all users
-GET /api/users/:id - Get user by ID
-PUT /api/users/profile - Update user profile

#Messages
-GET /api/messages/:chatId - Get messages for a chat
-POST /api/messages - Send a new message

#Chats
-POST /api/chats - Create new chat (individual or group)
-GET /api/chats - Get user's chats
-PUT /api/chats/group - Update group chat

#Deployment
The application is deployed on Vercel:
-Live Demo: https://swift-talk.vercel.app

#Deployment Steps:
-Connect your GitHub repository to Vercel
-Configure environment variables in Vercel dashboard
-Deploy automatically on git push

###License
This project is licensed under the MIT License.
