# React + Vite

Name: JANGAM PRASHANTH 
Company: CODTECH IT SOLUTIONS 
ID: CT08FEL Domain: Full Stack Development 
Duration: December 20 to January 20, 2025 
Mentor: SRAVANI

# Overview of the Project

Project: Recipe Sharing Platform

# Key Features of the Project:
Frontend:
React app powered by Vite for fast build and development.
React components will likely render views related to users and recipes.

- Frontend (React + Vite)
index.html: This is the entry point for the frontend. It includes the <div id="root"></div> element, where the React application will be rendered. The <script type="module" src="/src/main.jsx"></script> tag points to the main JavaScript file (main.jsx) that will be responsible for setting up the React application.
Vite is used as the build tool, which ensures fast development and efficient bundling for production.

Backend (Node.js + Express)
server.js: This is the entry point for the backend. It sets up an Express server with some important configurations:
dotenv: Loads environment variables from a .env file.
cors: Enables Cross-Origin Resource Sharing to allow the frontend to make requests to the backend.
express.json(): Middleware to parse incoming JSON requests.
express.static("public"): Serves static files from the public directory, which might include your frontend build files.
The server listens on a port (either the one defined in .env or 3000 by default) and sets up two routes (/ for general user routes and /recipe for recipe-related routes).
Database (MongoDB + Mongoose)
connectionDb.js: This module contains the logic to connect to MongoDB using Mongoose. It connects to the database using the connection string provided in the .env file. Once connected, a confirmation message is logged.


Backend:
Express server with routes for user and recipe data (/user and /recipe).
The server interacts with the frontend to handle requests and manage responses.
The public folder likely contains the compiled React files to be served by Express.
Database:

MongoDB database connection established via Mongoose.
The backend likely interacts with collections in MongoDB to store user and recipe data, though specific models and schemas are not visible here.
Routing:

The project has two routes:
/: Handles user-related actions (likely CRUD operations for users).
/recipe: Manages recipe-related data (likely CRUD for recipes).
Technologies Used:
React: Frontend framework for building the user interface.
Vite: Modern build tool to bundle and serve the React app.
Node.js & Express: Backend server handling API requests.
MongoDB & Mongoose: Database system to store and retrieve data.
dotenv: To manage environment variables securely.
CORS: To handle cross-origin requests between the backend and frontend.

# Output:

![screencapture-localhost-5173-2024-12-30-23_34_41](https://github.com/user-attachments/assets/35d5a64e-5ce9-419a-9397-b8f3c20227fd)

![screencapture-localhost-5173-myRecipe-2024-12-30-23_34_09](https://github.com/user-attachments/assets/06d0fd6d-e466-4dea-9655-0f80bfb42cd9)


![screencapture-localhost-5173-favRecipe-2024-12-30-23_34_30](https://github.com/user-attachments/assets/beee4a37-041f-481d-b626-dcb6fa282659)


This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
