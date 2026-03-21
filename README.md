# AI-MERN-Stack-Project

QuickGPT is a MERN-style AI assistant project with a React frontend and an Express/MongoDB backend in progress.

## Current Progress

The project currently includes:

- React client built with Vite
- Sidebar-based chat layout
- Recent chats list with search
- Community Images page
- Credit Plans page
- Login screen flow based on app context
- Dark mode support on the client
- Express server with MongoDB connection setup
- Basic root API route on the server

Some UI areas are still using dummy data and the backend routes are still in early setup.

## Tech Stack

- Frontend: React, Vite, React Router, Tailwind CSS
- Backend: Node.js, Express, MongoDB, Mongoose
- Other packages: Moment.js, React Markdown, Prism.js, JWT, bcryptjs

## Project Structure

```text
AI-MERN-Stack-Project/
├─ client/
│  ├─ public/
│  ├─ src/
│  │  ├─ assets/
│  │  ├─ components/
│  │  │  ├─ ChatBox.jsx
│  │  │  ├─ Message.jsx
│  │  │  └─ Sidebar.jsx
│  │  ├─ context/
│  │  │  └─ AppContext.jsx
│  │  ├─ pages/
│  │  │  ├─ Community.jsx
│  │  │  ├─ Credits.jsx
│  │  │  ├─ Loading.jsx
│  │  │  └─ Login.jsx
│  │  ├─ App.jsx
│  │  ├─ main.jsx
│  │  └─ index.css
│  ├─ package.json
│  └─ README.md
├─ server/
│  ├─ configs/
│  │  └─ db.js
│  ├─ .env
│  ├─ .gitignore
│  ├─ package.json
│  └─ server.js
└─ README.md
```

## Frontend Routes

- `/` - main chat screen
- `/credits` - credit plans page
- `/community` - community image gallery
- `/loading` - loading screen

## Run The Project

### Client

```bash
cd client
npm install
npm run dev
```

### Server

```bash
cd server
npm install
npm run server
```

## Environment

The server expects a MongoDB connection string in:

```env
MONGODB_URI=your_mongodb_connection_string
```

## Notes

- The client currently relies on context and dummy data for several screens.
- Server-side authentication, chat APIs, and image generation APIs are not fully wired yet.
- The project structure is ready for expanding into a complete MERN app.
