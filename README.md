# Notes App — MERN CRUD Lab

A full-stack Notes management app built with MongoDB, Express, React (Vite), and Node.js.

## Self Details
- Name: _Supriyo Ain_
- Roll Number: _2026202012_
- GitHub repository: _https://github.com/4insu/notes-app_

## Project Structure
```
notes-app/
|-- server/   # Express + Mongoose backend (port 5000)
|-- client/   # Vite + React frontend (port 5173)
```

## Prerequisites
- Node.js (v18+ recommended)
- A local MongoDB daemon running on `mongodb://localhost:27017`

## Setup & Run

### 1. Backend
```bash
cd server
npm install
npm start
```
Server starts on `http://localhost:5000` and connects to `mongodb://localhost:27017/notes_db`.

### 2. Frontend
In a separate terminal:
```bash
cd client
npm install
npm run dev
```
Client starts on `http://localhost:5173`.

## API Endpoints
| Method | Endpoint          | Description                     |
|--------|-------------------|----------------------------------|
| POST   | /api/notes        | Create a new note (201 Created)  |
| GET    | /api/notes        | Get all notes, newest first      |
| DELETE | /api/notes/:id    | Delete a note (200 OK / 404)     |

## Notes
- CORS is enabled on the server to allow requests from `http://localhost:5173`.
- Loading and empty states are handled in the UI.
- Screenshots of the running app (creation + deletion) go in `screenshots/`.