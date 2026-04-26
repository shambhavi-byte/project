# 🎬 StreamSphere API (Node.js + Express + MongoDB)

A production-grade backend API for a modern video-sharing and social media platform, combining YouTube-style video streaming with tweet/community post functionality.

Built using Node.js, Express, MongoDB, and Cloudinary, this project demonstrates scalable backend design, secure authentication, and real-world system architecture.

---

# 🚀 Core Features

## 🔐 Authentication & Security
- JWT-based authentication (Access + Refresh Tokens)
- Secure route protection using middleware

## 🎥 Video Platform
- Video upload & management (Cloudinary integration)
- Watch history tracking
- Channel profile system

## 💬 Social Features
- Comments system
- Likes system
- Subscriptions (follow channels)
- Tweet-style community posts

## 📊 Dashboard & Analytics
- Total videos, views, likes, subscribers
- Creator dashboard insights

## ⚙️ Backend Architecture
- Scalable MVC architecture
- Clean modular structure
- RESTful API design

---

# 🛠 Tech Stack

- Backend: Node.js, Express.js  
- Database: MongoDB, Mongoose  
- Authentication: JWT (Access + Refresh Tokens)  
- File Uploads: Multer  
- Cloud Storage: Cloudinary  
- Architecture: MVC Pattern  
- Version Control: Git & GitHub  

---

# 📂 Project Structure

controllers/   → Business logic  
models/        → Database schemas  
routes/        → API endpoints  
middlewares/   → Auth & file handling  
utils/         → Helper functions  

---

# 🔑 Authentication Flow

1. User registers  
2. User logs in  
3. Access token + Refresh token generated  
4. Access token used for protected APIs  
5. Refresh token used to regenerate access token  

---

# 📡 API Base URL

http://localhost:8000/api/v1

---

# ⚙️ Environment Variables

Create a `.env` file:

PORT=8000  
MONGODB_URI=your_mongodb_connection  

ACCESS_TOKEN_SECRET=your_secret  
REFRESH_TOKEN_SECRET=your_secret  

CLOUDINARY_CLOUD_NAME=  
CLOUDINARY_API_KEY=  
CLOUDINARY_API_SECRET=  

CORS_ORIGIN=http://localhost:3000  

---

# 📌 Major API Endpoints

## 👤 Users
POST /users/register  
POST /users/login  
POST /users/logout  

## 🎥 Videos
POST /videos/publish  
GET /videos  
GET /videos/:id  

## 💬 Comments
POST /comments/:videoId  
DELETE /comments/:commentId  

## 🔔 Subscriptions
POST /subscriptions/:channelId  

---

# 📊 Dashboard Analytics

- Total Videos  
- Total Views  
- Total Subscribers  
- Total Likes  

---

# 📦 Installation & Setup

git clone https://github.com/shambhavi-byte/streamsphere-api  
cd streamsphere-api  
npm install  
npm run dev  

Server runs at:  
http://localhost:8000  

---

# 🧠 Key Learnings

- Designing scalable REST APIs  
- Implementing secure JWT authentication  
- Handling media uploads & cloud storage  
- Structuring backend using MVC architecture  
- Working with MongoDB aggregation  

---

# 👩‍💻 Author

Shambhavi Gupta
