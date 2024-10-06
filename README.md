React Job Portal
This repository contains the backend and frontend code for a job portal application built using Node.js for the backend and React for the frontend. The backend handles data processing, authentication, and API services, while the frontend provides an interactive user interface for job seekers and employers.

Table of Contents
Project Structure
Features
Tech Stack
Getting Started
Backend Setup
Frontend Setup
Environment Variables
Scripts
Dependencies Overview
Backend Dependencies
Frontend Dependencies
Running the Application
License
Project Structure
The project is divided into two main parts:

Backend: A REST API server built using Express, which provides all the necessary services for the application, including authentication, database management, and file handling.
Frontend: A React-based single-page application (SPA) built using Vite that provides the user interface for job seekers and employers.
Features
Backend
User authentication (JWT-based)
File handling using Multer and Cloudinary for uploading images
Data storage using MongoDB
Secure password hashing with Bcrypt
RESTful API for handling CRUD operations
Frontend
Responsive job portal UI for users to register, login, search jobs, and manage profiles
State management using Redux Toolkit
Persistent storage for user sessions using Redux Persist
Interactive UI components using Radix UI
Routing for seamless navigation using React Router
Tech Stack
Backend: Node.js, Express, MongoDB
Frontend: React, Vite, Tailwind CSS
Authentication: JSON Web Tokens (JWT)
File Handling: Multer, Cloudinary
Getting Started
Backend Setup
Clone the repository:

bash
Copy code
git clone <repository-url>
cd backend
Install dependencies:

bash
Copy code
npm install
Create a .env file in the root directory with the required environment variables. See Environment Variables for more details.

Run the backend server in development mode:

bash
Copy code
npm run dev
Frontend Setup
Navigate to the frontend folder:

bash
Copy code
cd frontend
Install dependencies:

bash
Copy code
npm install
Run the frontend development server:

bash
Copy code
npm run dev
Environment Variables
For the backend, create a .env file in the root directory and add the following variables:

MONGO_URI: MongoDB connection string
JWT_SECRET: Secret key for signing JWT tokens
CLOUDINARY_CLOUD_NAME: Cloudinary account cloud name
CLOUDINARY_API_KEY: Cloudinary API key
CLOUDINARY_API_SECRET: Cloudinary API secret
Scripts
Backend Scripts
npm run dev: Starts the backend server using Nodemon for live-reloading.
npm test: Placeholder for running tests.
Frontend Scripts
npm run dev: Starts the development server for the frontend.
npm run build: Builds the production version of the frontend.
npm run lint: Runs ESLint to check for code quality issues.
npm run preview: Previews the production build.
Dependencies Overview
Backend Dependencies
bcryptjs: Used for hashing user passwords.
cloudinary: Cloud service for managing images.
cookie-parser: Parses cookies for user sessions.
cors: Handles Cross-Origin Resource Sharing.
datauri: Converts files to Data URI format for easier file handling.
dotenv: Loads environment variables from a .env file.
express: Web framework for building REST APIs.
jsonwebtoken: For user authentication using JSON Web Tokens.
mongoose: ODM for MongoDB.
multer: Middleware for handling file uploads.
nodemon: Utility for automatically restarting the server during development.
Frontend Dependencies
@radix-ui/react- components*: Set of UI components used for building accessible UI elements.
@reduxjs/toolkit & react-redux: State management for managing user sessions, data, and application state.
axios: Promise-based HTTP client for making API requests.
embla-carousel-react: A carousel library for displaying items like job listings.
framer-motion: For adding animations to the user interface.
lodash: Utility library for data manipulation.
react-router-dom: Routing library for navigation.
redux-persist: For persisting the Redux state to local storage.
tailwindcss: Utility-first CSS framework for styling.
vite: Build tool that provides fast development server for the frontend.
Frontend Dev Dependencies
@vitejs/plugin-react: Vite plugin for React support.
eslint & related plugins: Linting tools for maintaining code quality.
postcss & autoprefixer: Used for CSS processing and compatibility.
Running the Application
To run the complete application:

Start the Backend Server:

Navigate to the backend folder and run:
bash
Copy code
npm run dev
Start the Frontend Server:

Navigate to the frontend folder and run:
bash
Copy code
npm run dev
The backend will typically be available on http://localhost:5000 and the frontend on http://localhost:5173.