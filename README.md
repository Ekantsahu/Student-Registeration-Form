# Student Registration Form

A simple student registration form built with HTML, CSS, and a small Node.js server. This repository contains the frontend form (`form.html` and `form.css`) and a minimal server (`server.js`) to serve the page or handle form submissions.

## Features

- Simple responsive registration form UI
- Static CSS styling in `form.css`
- Minimal Node.js server in `server.js` for local testing
- Stores submitted registrations in a MongoDB database (database name: `students`).

## Prerequisites

- Node.js (v12+ recommended)
- npm (comes with Node.js)
- MongoDB server (local) or MongoDB Atlas
- MongoDB Compass (optional) — used to view the `students` database and its collections

## Quick start (Windows PowerShell)

1. Install dependencies (if any listed in `package.json`):

```powershell
npm install
```

2. Start the server (if `server.js` is the server file):

```powershell
# (Optional) set the MongoDB connection string, then start the server.
# Example for a local MongoDB instance (database name `students`):
$env:MONGODB_URI = "mongodb://localhost:27017/students"
node server.js

# Or use a MongoDB Atlas connection string (replace <your-uri>):
$env:MONGODB_URI = "<your-mongodb-atlas-connection-string>"
node server.js
```

3. Open the form in your browser:

- If the server serves the page, open `http://localhost:3000` (or the port shown in the server logs).
- Or open `form.html` directly by double-clicking it or using your browser's Open File dialog.

## Repository files

- `form.html` — The registration form markup.
- `form.css` — Styles for the form.
- `server.js` — Minimal Node.js server to serve the form or accept submissions.
- `package.json` — Project metadata and scripts.

## Database

- The app stores registrations in a MongoDB database named `students`.
- You can inspect data using MongoDB Compass by connecting to your MongoDB instance and opening the `students` database.

## Notes

- If you want me to add a `start` script to `package.json` (for `npm start`) or add instructions for building/deploying, tell me and I can update the repo.

- The server reads the `MONGODB_URI` environment variable to connect to MongoDB. If you want, I can add a `.env` example and `dotenv` support.


Created for the Student Registration Form project.
