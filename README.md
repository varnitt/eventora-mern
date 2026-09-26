Eventora — MERN Event Management Platform

Eventora is a full-stack MERN event management platform designed to make discovering, creating, and managing events simple and secure.

The platform includes user authentication, event discovery, event bookings, and role-based access control, providing different capabilities based on the user's role.

✨ Features

🔐 User Authentication

User registration and login

Protected routes

Secure authentication flow

🎫 Event Management

Create and manage events

View event details

Discover available events

🔎 Event Discovery

Browse events

View event information and availability

Find events relevant to users

📅 Event Booking

Book events

Manage booking-related information

Prevent unauthorized booking actions

🛡️ Role-Based Access Control

Different permissions for different user roles

Protected administrative/event-management operations

Server-side authorization checks

🌐 Full-Stack Architecture

React frontend

Node.js + Express backend

MongoDB database

REST API communication

🛠️ Tech Stack

Frontend

React.js

JavaScript

HTML5

CSS3

Backend

Node.js

Express.js

REST APIs

Authentication & authorization

Database

MongoDB

Mongoose

Development Tools

Git & GitHub

npm

VS Code

🏗️ Architecture

┌──────────────────────┐
│      React Client    │
│   UI / User Actions  │
└──────────┬───────────┘
           │ HTTP / REST API
           ▼
┌──────────────────────┐
│   Express + Node.js  │
│ Routes / Controllers │
│ Middleware / Auth    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│       MongoDB        │
│   Event / User /     │
│   Booking Data       │
└──────────────────────┘

📁 Project Structure

A typical structure for the project is:

Eventora-MERN-main/
│
├── frontend/
│   ├── src/
│   └── package.json
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   └── package.json
│
├── .gitignore
└── README.md

Folder names may vary slightly depending on the current project structure.

⚙️ Getting Started

1. Clone the repository

git clone https://github.com/varnitt/eventora-mern.git
cd eventora-mern

2. Install dependencies

Install dependencies for both the frontend and backend.

cd frontend
npm install

cd ../backend
npm install

3. Configure environment variables

Create a .env file inside the backend directory.

Example:

PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

Use the environment variables required by the current backend configuration.

4. Start the backend

cd backend
npm run dev

5. Start the frontend

Open another terminal:

cd frontend
npm start

The exact frontend command may differ if the project uses Vite or another React setup.

🔐 Authentication & Authorization

Eventora separates authentication from authorization:

Authentication determines who the user is.

Authorization determines what that user is allowed to do.

Protected backend routes use authentication middleware, while role-based checks restrict operations according to the user's permissions.

This prevents users from accessing management functionality simply by calling the API directly from the client.

🔄 Application Flow

A typical booking flow looks like:

User
  │
  ▼
Login / Register
  │
  ▼
Authentication
  │
  ▼
Browse Events
  │
  ▼
Select Event
  │
  ▼
Book Event
  │
  ▼
Backend Validation
  │
  ▼
MongoDB
  │
  ▼
Booking Confirmation

🚀 Future Improvements

Potential improvements for the platform include:

Payment gateway integration

Email notifications

Event search and advanced filtering

Event categories

Pagination

Organizer dashboards

Booking history

Event analytics

Image/file uploads

Automated testing

API documentation with Swagger/OpenAPI

Deployment with CI/CD

📌 Project Goals

The main goal of Eventora is to demonstrate how a modern MERN application can combine:

Frontend development

REST API design

Database modeling

Authentication

Authorization

Role-based access control

Event and booking workflows

Full-stack application architecture

👨‍💻 Author

Varnitt

GitHub: https://github.com/varnitt

⭐ If you find the project useful, consider giving the repository a star.
