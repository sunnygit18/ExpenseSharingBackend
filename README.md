# Expense Sharing Backend

A RESTful backend application designed to simplify expense sharing among users and groups. The project provides APIs for managing users, groups, shared expenses, balances, and settlements using Node.js, Express.js, and MongoDB Atlas.

---

## 🚀 Features

- **User Management** — APIs for managing users.
- **Group Management** — Organize users into groups for shared expenses.
- **Expense Tracking** — Manage expenses through dedicated REST APIs.
- **Balance Management** — Access balance information between users.
- **Settlement Management** — Dedicated APIs for handling settlements.
- **Database Integration** — Persistent data storage using MongoDB Atlas.
- **Health Monitoring** — A health-check endpoint to verify server responsiveness.

---

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB Atlas
- **ODM:** Mongoose
- **Environment Configuration:** dotenv
- **Development Tool:** Nodemon
- **API Architecture:** RESTful APIs

---

## 📂 Project Structure

```text
expenseSharing-backendSunny/
├── src/
│   ├── config/
│   │   └── DB.js
│   ├── routes/
│   │   ├── user.routes.js
│   │   ├── group.routes.js
│   │   ├── expense.routes.js
│   │   ├── balance.routes.js
│   │   └── settlement.routes.js
│   └── app.js
├── index.js
├── package.json
├── package-lock.json
├── .gitignore
└── README.md
```

---

## ⚙️ Setup & Installation

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd expenseSharing-backendSunny
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file in the root directory:

```env
PORT=3001
MONGO_URI=your_mongodb_connection_string
```

Replace the placeholder with your MongoDB Atlas connection string. Never commit your actual `.env` file or database credentials to GitHub.

### 4. Run the application

Start the development server:

```bash
npm run dev
```

Or start it normally:

```bash
npm start
```

The server will run at:

`http://localhost:3001`

---

## 📌 API Overview

| Endpoint | Purpose |
|---|---|
| `GET /` | Check the backend welcome message |
| `GET /health` | Verify server responsiveness |
| `/api/users` | User management |
| `/api/groups` | Group management |
| `/api/expenses` | Expense management |
| `/api/balances` | Balance management |
| `/api/settlements` | Settlement management |

For supported HTTP methods and individual operations, refer to the corresponding route files.

---

## 🧠 Engineering Highlights

- **Modular Architecture** — Separates application setup, database configuration, and route handling.
- **Dedicated API Routes** — Keeps user, group, expense, balance, and settlement endpoints organized.
- **Database Connectivity** — Connects the application to MongoDB Atlas through Mongoose.
- **Environment-Based Configuration** — Keeps configuration values outside the application source code.
- **Server Health Check** — Provides a lightweight endpoint for checking server responsiveness.

---

## 🔮 Future Improvements

- JWT-based authentication and authorization
- Flexible expense splitting by percentage or custom amounts
- Automated balance calculation and settlement recommendations
- Input validation and centralized error handling
- API documentation using Swagger
- Unit and integration testing

---

## 👨‍💻 Author

**Sunny Kumar**