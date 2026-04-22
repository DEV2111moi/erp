# 🚀 Procurement ERP with AI Quote Evaluation Engine

> *“The process never ends — it evolves until intelligence itself fades.”*

A modern **Procurement ERP System** designed to streamline vendor management, RFQ handling, and intelligent decision-making using a **rule-based AI evaluation engine**.

---

## 🧠 Overview

This ERP system simplifies the procurement lifecycle:

- 📄 Create and manage **RFQs (Request for Quotations)**
- 🏢 Handle multiple **vendors & quotes**
- ⚡ Automatically evaluate quotes using an **AI-powered scoring engine**
- 📊 Make **data-driven purchasing decisions**

---

## 🎯 Key Feature: AI Quote Evaluation Engine

The core innovation of this project is the **AI Quote Evaluation Engine** — a smart scoring system that analyzes vendor quotes and ranks them.

### 🔍 Problem Solved
Comparing multiple vendor quotes manually is:
- Time-consuming ⏳  
- Error-prone ❌  
- Inefficient 📉  

### 💡 Solution
A **rule-based AI system** that:
- Evaluates each quote
- Scores based on key factors
- Recommends the best vendor automatically

---

## ⚙️ How AI Scoring Works

Each quote is evaluated using **3 weighted factors**:

| Factor        | Weight | Description                     |
|--------------|--------|---------------------------------|
| 💰 Price      | 50%    | Lower price = higher score     |
| 🚚 Delivery   | 30%    | Faster delivery = better       |
| ⭐ Rating     | 20%    | Higher vendor rating preferred |

### 🧮 Formula Logic (Simplified)

- Price Score = Min Price / Vendor Price  
- Delivery Score = Min Delivery / Vendor Delivery  
- Rating Score = Vendor Rating / Max Rating  

Final Score:

AI Score = (0.5 × Price) + (0.3 × Delivery) + (0.2 × Rating)

---

## 🔄 Workflow

1. Admin selects an RFQ  
2. Clicks **“Run AI Evaluation”**  
3. Backend:
   - Fetches quotes & vendor data  
   - Runs scoring algorithm  
   - Stores `aiScore`  
4. Frontend displays:
   - Ranked vendors  
   - Best quote per product  

---

## 🏗️ Tech Stack

### 💻 Frontend
- React.js
- Axios
- Bootstrap / UI Components

### 🔧 Backend
- Node.js
- Express.js

### 🗄️ Database
- MongoDB (Mongoose)

### 🔐 Authentication
- JWT-based Auth
- Role-Based Access Control (Admin)

---

## 📁 Project Structure

moidev/
│
├── backend/
│   ├── config/
│   │   └── db.js              # Database connection
│   │
│   ├── middleware/
│   │   ├── auth.js           # Authentication middleware
│   │   └── role.js           # Role-based access control
│   │
│   ├── models/               # Data models (RFQ, Vendor, User, etc.)
│   ├── routes/               # API routes
│   ├── seed/                 # Sample data
│   │
│   ├── services/
│   │   └── aiEngine.js       # AI logic for quote comparison
│   │
│   ├── server.js             # Backend entry point
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── api/
│   │   │   └── axios.js      # Axios configuration
│   │   │
│   │   ├── components/
│   │   │   └── Sidebar.jsx   # UI components
│   │   │
│   │   ├── context/          # Global state management
│   │   ├── pages/            # Application pages
│   │   │
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   │
│   ├── index.html
│   ├── vite.config.js
│   └── package.json
│
└── README.md
```

## 🔄 System Workflow

```
Admin Login
   ↓
Create RFQ (Multiple Products)
   ↓
Select Vendors
   ↓
Vendors Receive RFQ
   ↓
Vendors Submit Quotes
   ↓
System Stores Data
   ↓
AI Compares Quotes
   ↓
Admin Reviews Suggestions
   ↓
Generate Purchase Order
   ↓
Order Completion
```

## ⚙️ Installation & Setup

### 🔧 Prerequisites
- Node.js
- npm
- MongoDB

### 📥 Clone Repository
```bash
git clone https://github.com/your-username/procurement-erp.git
cd procurement-erp
```

### 🔙 Backend Setup
```bash
cd backend
npm install
npm start
```

### 🌐 Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

## 🔐 Environment Variables

Create a `.env` file in `backend/`:

```
PORT=5000
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_secret_key
```

## 🤖 AI Engine

Located in: `backend/services/aiEngine.js`

Used for:
- Quote comparison
- Vendor ranking
- Decision support
