# 🎬 YouTube Backend API (Node.js + Express + MongoDB)

A production-style backend API inspired by YouTube, built with **Node.js, Express, MongoDB, and Cloudinary**.
This project implements authentication, video management, playlists, subscriptions, likes, comments, and dashboard analytics.

---

# 🚀 Features

* User Authentication (JWT + Refresh Tokens)
* Video Upload with Cloudinary
* Comments System
* Likes System
* Playlist Management
* Channel Subscriptions
* Watch History
* Dashboard Analytics
* Secure API using Middleware

---

# 🛠 Tech Stack

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT Authentication
* Multer
* Cloudinary
* REST APIs

---

# 📂 Project Architecture

MVC Architecture

controllers → Business logic
models → MongoDB schema
routes → API endpoints
middlewares → authentication & uploads
utils → reusable utilities

---

# 🔑 Authentication Flow

1. User registers
2. User logs in
3. Access token + refresh token generated
4. Access token used for protected routes
5. Refresh token used to generate new access tokens

---

# 📡 API Base URL

```
http://localhost:8000/api/v1
```

---

# ⚙️ Environment Variables

Create `.env` file

```
PORT=8000
MONGODB_URI=your_mongodb_connection
ACCESS_TOKEN_SECRET=your_secret
REFRESH_TOKEN_SECRET=your_secret

CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=

CORS_ORIGIN=http://localhost:3000
```

---

# 📌 Major API Endpoints

Users
POST /users/register
POST /users/login
POST /users/logout

Videos
POST /videos/publish
GET /videos
GET /videos/:id

Comments
POST /comments/:videoId
DELETE /comments/:commentId

Subscriptions
POST /subscriptions/:channelId

---

# 📊 Dashboard Analytics

* Total videos
* Total views
* Total subscribers
* Total likes

---

# 📦 Installation

```
git clone https://github.com/yourusername/youtube-backend
cd youtube-backend
npm install
npm run dev
```

Server will run on:

```
http://localhost:8000
```

---

# 🧠 Learning Outcomes

* REST API Design
* Authentication using JWT
* File Upload Handling
* Cloud Storage Integration
* MongoDB Aggregation
* Backend Architecture

---

# 👩‍💻 Author

Shambhavi Gupta
