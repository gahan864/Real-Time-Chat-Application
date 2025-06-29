# XeroxChat – Real-Time Socket.IO Chat App

XeroxChat is a real-time chat application built using Node.js, Express, and Socket.IO. It supports multi-user chat rooms with user join/leave notifications, message broadcasting, and a simple front-end.

---

## 🚀 Features

- Real-time messaging with Socket.IO
- Room-based chat (join any room)
- User join and leave notifications
- Simple UI served via Express static hosting
- Timestamps on messages (via moment-timezone)
- Lightweight and easy to extend

---

## 📦 Tech Stack

| Layer        | Technology         |
|--------------|--------------------|
| Backend      | Node.js + Express  |
| Real-Time    | Socket.IO          |
| Frontend     | Vanilla HTML/CSS/JS (served via Express) |
| Time utility | moment-timezone    |

---

## 📁 Project Structure

```

chat-server/
├── app.js                 # Main server logic
├── package.json           # Dependencies & scripts
├── public/                # Frontend HTML/CSS/JS
├── utils/
│   ├── messages.js        # Format chat messages with timestamp
│   └── users.js           # Manage users per room (join, leave, etc.)

````

---

## ⚙️ Getting Started

1. Clone the repository:

```bash
git clone https://github.com/yourusername/xerox-chat.git
cd xerox-chat
````

2. Install dependencies:

```bash
npm install
```

3. Start the server:

```bash
npm start
```

4. Open your browser at:

```
http://localhost:3000
```

---

## 🧠 How It Works

* Users enter a username and room name to join.
* Upon joining, they receive a welcome message and others in the room are notified.
* All chat messages are broadcasted to everyone in the room.
* User disconnection is broadcasted to others.
* All state (users, rooms) is managed in memory using utils/users.js.

---

## 📷 UI Preview

> Add screenshots of the chat interface or the public/index.html if you wish.

---

## 🛠️ Future Improvements

* Add persistent chat history (MongoDB)
* Add JWT authentication
* Add profanity filtering (RoBERTa or Perspective API)
* Deploy to Render, Railway, or AWS

---

## 📄 License

This project is licensed under the ISC License.

```
