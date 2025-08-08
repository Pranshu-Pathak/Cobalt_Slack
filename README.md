# Slack Connect – Refold Intern Assignment

## 📌 Project Overview
Slack Connect is a full-stack web application that allows users to:
- Connect their Slack workspace using OAuth 2.0.
- Send messages to any Slack channel instantly.
- Schedule messages to be delivered at a later time.
- Manage (view/cancel) scheduled messages from a single dashboard.

This project was developed as part of the Refold Internship Assignment to demonstrate OAuth integration, secure token management, and reliable message scheduling.

---

## 🚀 Core Features

### ✅ OAuth 2.0 Integration
- Securely connects a user's Slack workspace.
- Stores `access_token` and `refresh_token` securely.
- Automatically refreshes tokens when expired to maintain access.

### ✉️ Message Sending
- Select a Slack channel.
- Compose and send a message instantly.

### ⏰ Scheduled Messaging
- Schedule a message for future delivery.
- Messages are stored in a persistent store and dispatched at the scheduled time.

### 📋 Scheduled Message Management
- View all upcoming scheduled messages.
- Cancel any message before it is sent.

---

## ⚙️ Tech Stack

- **Frontend**: React.js, TypeScript, JavaScript (ES6+)
- **Backend**: Node.js, Express.js (TypeScript)
- **Database**: MongoDB / JSON / SQLite (based on setup)
- **Authentication**: OAuth 2.0 (Slack)

---

## 🧱 Architecture Overview

- **OAuth Flow**: Handles authorization and token exchange using Slack's OAuth 2.0.
- **Token Management**: Access & refresh tokens are stored securely and refreshed automatically when expired.
- **Message Scheduler**: Backend checks pending messages and sends them at the scheduled time.
- **Persistence**: All scheduled messages and tokens are stored reliably to ensure consistent operation.

---

## 📚 Challenges & Learnings

- Handling **token expiry** and implementing a smooth **refresh token mechanism** without affecting user experience.
- Building a **robust message scheduler** that works even across restarts or server downtime.
- Ensuring **reliable UI feedback** and smooth UX for message creation, scheduling, and cancellation.
- Working with **Slack API rate limits** and proper error handling.

---

## 📎 Repository Structure

```
/frontend
  ├── components/
  ├── pages/
  └── ... (React app files)

/backend
  ├── routes/
  ├── services/
  ├── utils/
  └── server.ts

/shared
  └── (Shared types or constants)

.env.example
README.md
```

---

## 📄 License

This project is provided for assessment and educational purposes only.
