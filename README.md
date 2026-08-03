# 🚀 OpenConnect – Secure Real-Time Messaging & Video Calling Platform

> **OpenConnect** is a modern, full-stack real-time communication platform that provides secure messaging, high-quality audio/video calling, and seamless collaboration. Built with **React, Node.js, Express, MongoDB, Socket.io, and WebRTC**, it combines low-latency communication with robust authentication, end-to-end encryption, and a clean, responsive user experience.

---

# 📖 Overview

OpenConnect is designed to demonstrate how modern communication platforms such as **WhatsApp, Microsoft Teams, Discord, and Google Meet** work under the hood.

The application supports:

* Secure one-to-one messaging
* Group conversations
* High-quality voice and video calls
* Real-time notifications
* End-to-End Encryption (E2EE)
* Media sharing
* JWT & Google OAuth authentication
* Online presence tracking
* Modern responsive UI

The project focuses on **real-time systems**, **security**, **peer-to-peer communication**, and **scalable backend architecture**.

---

# ✨ Key Features

## 🔐 Secure Authentication

* JWT-based authentication
* Google OAuth login
* Password hashing using bcrypt
* Protected API routes
* Secure session management

---

## 💬 Real-Time Messaging

* One-to-one chat
* Group chats
* Instant message delivery
* Typing indicators
* Read receipts
* Message status updates
* Chat history synchronization

---

## 📞 Audio & Video Calling

* WebRTC peer-to-peer communication
* Crystal-clear audio calls
* HD video calls
* Low latency communication
* Automatic ICE candidate exchange
* STUN/TURN server support

---

## 🔒 End-to-End Encryption (E2EE)

Private chats are encrypted using **AES-GCM encryption**.

Encryption keys are generated locally using the **Web Crypto API**, ensuring that:

* Messages remain encrypted during transmission.
* The server stores only encrypted content.
* Only the sender and receiver can decrypt messages.

---

## 📸 Media Sharing

* Image uploads
* File sharing
* Cloudinary integration
* Secure media storage

---

## 🟢 Presence System

* Online/offline status
* Last seen
* Active user tracking
* Real-time presence updates

---

## 🚫 Privacy Controls

* Block users
* Unblock users
* Privacy management
* Secure conversations

---

## 🎨 Premium User Interface

* Fully responsive design
* Dark mode support
* Clean chat interface
* Modern animations
* Mobile-friendly layout

---

# 🛠 Tech Stack

## Frontend

* React (Vite)
* Tailwind CSS
* Headless UI
* Heroicons
* Socket.io Client
* Axios
* React Router
* Web Crypto API

---

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* Socket.io
* JWT Authentication
* bcrypt
* Multer
* Cloudinary

---

## Real-Time Technologies

* Socket.io
* WebRTC
* STUN
* TURN
* ICE Candidates

---

## Optional Scaling

* Redis Socket.io Adapter
* Docker
* Docker Compose

---

# 🏗 System Architecture

```text
                     Users
                        │
                        ▼
            React Frontend (Vite)
                        │
         ┌──────────────┴──────────────┐
         │                             │
         ▼                             ▼
REST APIs (HTTP)               Socket.io (WebSocket)
(Login, Users, Media)      Messaging, Presence, Signaling
         │                             │
         └──────────────┬──────────────┘
                        ▼
             Node.js + Express Server
                        │
        ┌───────────────┼────────────────┐
        │               │                │
        ▼               ▼                ▼
 JWT Middleware   Business Logic   Socket.io Server
        │               │                │
        └───────────────┴────────────────┘
                        │
                        ▼
                   MongoDB Database
                        │
                        ▼
          Users • Chats • Messages • Groups
```

---



# 📂 Database Design

## Users

* User Profile
* Authentication
* Last Seen
* Online Status
* Blocked Users

---

## Chats

* Participants
* Last Message
* Chat Type
* Updated Time

---

## Messages

* Sender
* Receiver
* Encrypted Message
* Read Status
* Timestamp

---

## Groups

* Group Name
* Members
* Admin
* Created Date

---

# 🔥 REST APIs

Authentication

```
POST /api/auth/register
POST /api/auth/login
GET  /api/auth/profile
```

Users

```
GET /api/users
PUT /api/users/profile
POST /api/users/block
```

Chats

```
GET /api/chats
POST /api/chats
GET /api/messages/:chatId
POST /api/messages
```

Calls

```
POST /api/call/start
POST /api/call/end
```

Media

```
POST /api/upload
```

---

# 🔒 Security Features

* JWT Authentication
* Google OAuth
* bcrypt Password Hashing
* End-to-End Encryption
* AES-GCM Encryption
* Protected Routes
* Input Validation
* Secure File Uploads
* CORS Protection
* Environment Variables
* HTTPS Ready

---

# ⚡ Performance Optimizations

* WebSocket-based real-time communication
* Peer-to-peer media transfer
* Optimized MongoDB schemas
* Efficient Socket.io event handling
* Lazy loading of chat history
* Cloudinary CDN for media delivery
* Optional Redis adapter for Socket.io scaling



---

# 🚀 Future Enhancements

* AI-powered smart replies
* AI meeting summaries
* Speech-to-text transcription
* Multi-language translation
* Screen sharing
* Voice notes
* Video call recording
* Push notifications
* Message scheduling
* Disappearing messages
* Multi-device synchronization
* End-to-end encrypted group chats

---


# 📜 License

This project is licensed under the **MIT License**.

---

# 👨‍💻 Author

**Sk Sadiya Parvin**

* GitHub: https://github.com/sksadiya22

---

⭐ If you found this project useful, consider giving it a **Star** on GitHub!
