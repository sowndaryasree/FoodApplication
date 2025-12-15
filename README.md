# 🍽️ Foodiee — Full-Stack Food Delivery Application

*A full‑stack MERN project.*

---

## 🚀 Project Overview

Foodiee is a full-stack food delivery web application where users can browse menu items, add items to a cart, authenticate (login/register), and place orders. The repository contains a complete frontend (React) and backend (Node/Express + MongoDB) implementation.

---

## 📂 Repository Structure

```
upskillcampus/
│
├── backend/                # Server-side code (Node + Express + MongoDB)
│   ├── config/             # Database connection, environment setup
│   ├── middleware/         # Auth middleware (JWT verification)
│   ├── models/             # Mongoose schemas (User, FoodItem, Order)
│   ├── routes/             # API routes (auth, food, cart, orders)
│   ├── package.json        # Backend dependencies & scripts
│   └── server.js           # App entry point
│
├── frontend/               # Client-side React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # App pages (Home, Login, Cart, Checkout)
│   │   ├── context/        # Global state (Auth, Cart)
│   │   ├── App.js          # Routes & layout
│   │   └── index.js        # React entry
│   ├── public/             # Static assets (favicon, index.html)
│   └── package.json        # Frontend dependencies & scripts
│
├── .gitignore
└── README.md
```

---

## 🔧 Tech Stack

* **Frontend:** React, React Router, Context API, Axios
* **Backend:** Node.js, Express, MongoDB (Mongoose), JWT, bcryptjs
* **Dev Tools:** nodemon (dev), dotenv

---

## 🌟 Key Features

* **Authentication:** Register / Login with JWT-based protected routes.
* **Menu browsing:** List food items with categories and details.
* **Cart & Checkout:** Add/remove items, place orders.
* **Order history:** Users can view their past orders.
* **Admin utilities (optional):** Add/edit/delete menu items and manage orders.

---

## 🛠️ Local Setup (Run locally)

### 1) Backend

```bash
cd backend
npm install
# create a .env file with the following keys:
# MONGODB_URL=<your_mongo_connection_string>
# JWT_SECRET=<a_secure_secret>
# PORT=5000
npm start
```

### 2) Frontend

```bash
cd frontend
npm install
npm start
```

Open the app at `http://localhost:3000` and the backend API at `http://localhost:5000`.

---

## 📦 Important Notes

* `node_modules/` are intentionally excluded. Do **not** push `node_modules` to the repo.
* Keep `.env` values secret — do not commit them.

---

## 📜 Useful Scripts

**Frontend**

```bash
npm start      # start dev server
npm run build  # build production bundle
```

**Backend**

```bash
npm start      # start server
npm run dev    # start with nodemon (auto-reload)
```
