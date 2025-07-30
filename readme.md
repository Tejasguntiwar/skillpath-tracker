
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
