
# MERN Stack Blog App

A full-featured blog platform built with **MongoDB, Express, React, and Node.js**. This repository contains both the frontend and backend code in a single monorepo structure.

## 📂 Project Structure

```text
MERN-Stack-Blog-app/
├── client/          # React Frontend (Vite/CRA)
├── server/          # Node.js/Express Backend
├── .gitignore
└── README.md
🚀 Quick Start
Prerequisites
Node.js >= 16.x
MongoDB instance (Local or Atlas URI)
1. Clone & Install
Since this is a monorepo, you need to install dependencies for both folders separately.

bash

Copy
git clone https://github.com/rupam121/MERN-Stack-Blog-app.git
cd MERN-Stack-Blog-app

# Install Backend Dependencies
cd server && npm install && cd ..

# Install Frontend Dependencies
cd client && npm install && cd ..
2. Environment Variables
Create a .env file inside the server folder:

env

Copy
# server/.env
PORT=5000
MONGO_URI=mongodb+srv://<user>:<pass>@cluster.mongodb.net/blogdb
JWT_SECRET=your_super_secret_key
Create a .env file inside the client folder:

env

Copy
# client/.env
VITE_API_URL=http://localhost:5000/api
3. Run the Application
You need to run two terminals simultaneously.

Terminal 1 (Backend):

bash

Copy
cd server
npm run dev
Terminal 2 (Frontend):

bash

Copy
cd client
npm run dev
Note: If you are using Create React App instead of Vite, the frontend command will be npm start.

🛠️ Tech Stack
React 18
Node.js
Redux Toolkit / Context
Express.js
Axios
Mongoose (ODM)
Tailwind CSS / MUI
JWT & Bcryptjs
React Router v6
Multer (Image Uploads)
🔑 Key Features
Auth System: Secure JWT registration & login
Blog CRUD: Create, Edit, Delete posts with Rich Text Editor
Interactions: Comments and Likes system
Media: Profile pictures and blog cover images
State Management: Global state for user session & theme

📡 API Endpoints
POST
/api/auth/register
Register new user
Public
POST
/api/auth/login
Login user
Public
GET
/api/posts
Get all posts
Public
POST
/api/posts
Create new post
Protected
PUT
/api/posts/:id
Update post
Owner Only
DELETE
/api/posts/:id
Delete post
Owner Only
POST
/api/comments
Add comment
Protected

🚢 Deployment
Backend
Recommended: Render / Railway / Heroku
Set environment variables in your hosting dashboard
Ensure MONGO_URI uses your production database
Frontend
Recommended: Vercel / Netlify
Set build command: npm run build
Set output directory: dist (Vite) or build (CRA)
Add VITE_API_URL env variable pointing to your deployed backend URL

🤝 Contributing
Fork the Project
Create your Feature Branch (git checkout -b feature/AmazingFeature)
Commit your Changes (git commit -m 'Add some AmazingFeature')
Push to the Branch (git push origin feature/AmazingFeature)
Open a Pull Request
📄 License
Distributed under the MIT License. See LICENSE for more information.

👤 Author
Rupam

GitHub: @rupam121
