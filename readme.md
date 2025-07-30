
1️⃣ File & Folder Structure Planning (No Code Yet)

skillpath-tracker/
/backend → REST APIs, MongoDB, auth logic

/frontend → React UI, routes, dashboards

-------------------------------------------------------------------------------------------------

2️⃣ Backend Folder Structure

backend/
├── server.js                # Entry point
├── config/
│   └── db.js                # MongoDB connection logic
├── controllers/
│   ├── authController.js    # Register/Login logic
│   └── goalController.js    # CRUD for goals
├── middleware/
│   ├── authMiddleware.js    # JWT verification
│   └── errorMiddleware.js   # Error handler
├── models/
│   ├── User.js              # Mongoose user schema
│   └── Goal.js              # Mongoose goal schema
├── routes/
│   ├── authRoutes.js        # POST /register, /login
│   └── goalRoutes.js        # GET/POST/PUT/DELETE goals
└── .env                     # Secrets like MONGO_URI, JWT_SECRET

-------------------------------------------------------------------------------------------------

3️⃣ Frontend Folder Structure

frontend/
├── src/
│   ├── components/         # Navbar, ProtectedRoute, GoalCard
│   ├── pages/              # Home, Login, Register, Dashboard
│   ├── App.jsx             # All routes
│   ├── api.js              # Axios config
│   └── styles/             # Tailwind or CSS
├── public/index.html
└── .env                   # VITE_API_URL (backend URL)

-------------------------------------------------------------------------------------------------

4️⃣ Tools to Set Up

🧰 Backend:
npm init -y

Install: express, mongoose, cors, dotenv, bcryptjs, jsonwebtoken, nodemon

🧰 Frontend:
npm create vite@latest (React + JS template)

Install: axios, react-router-dom, tailwindcss (optional), react-icons

-------------------------------------------------------------------------------------------------

✅ Initial Git Setup (Local Repo)

🧩 Step 0: Initialize Git in the root folder

Assuming your project is in skillpath-tracker:

cd path/to/skillpath-tracker
git init

🧩 Step 1: Create .gitignore
Before adding files, make sure you ignore unnecessary stuff:

📄 In your root project directory, create a file named .gitignore and add this:

# Node modules
node_modules/
# Build output
dist/
build/
# Logs
*.log
# Env files
.env
.env.*
# System
.DS_Store
Thumbs.db
# IDE
.vscode/
.idea/

👉 Git command:

git add .gitignore
git commit -m "chore: add .gitignore"

🧩 Step 2: First Commit (basic folders and setup)
After you've created all folders and installed packages:

git add .
git commit -m "Initial Commit: project setup with frontend/backend folders and libraries"

-------------------------------------------------------------------------------------------------

🚀 Optional: Connect to GitHub
If you want to push your project online:

Create a new repository on GitHub (e.g., skillpath-tracker)

Run this in your local project root:

git remote add origin https://github.com/your-username/skillpath-tracker.git
git branch -M main
git push -u origin main