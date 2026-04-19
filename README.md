# 🏢 Procurement ERP System

## 📌 Overview

This project is a Procurement ERP (Enterprise Resource Planning) System designed to automate and streamline the purchasing process within an organization.

It enables admins to create RFQs, vendors to submit quotations, and the system to analyze and compare quotes for efficient decision-making.

## 🚀 Key Features

### 🔐 Authentication & Role-Based Access
- Secure login system (Admin / Vendor)

### 📄 RFQ (Request for Quotation) Management
- Admin can create RFQs for multiple products
- Send RFQs to selected vendors

### 💰 Vendor Quotation System
- Vendors submit quotes for requested products

### 🤖 AI-Based Quote Comparison
- AI engine analyzes and compares vendor quotations

### 📦 Purchase Order Generation
- Admin can generate PO based on best quote

### 📊 Data Management
- Organized storage of RFQs, quotes, and transactions

## 🏗️ Tech Stack

### Frontend
- React (Vite)
- CSS / Tailwind
- Axios (API communication)

### Backend
- Node.js
- Express.js

### Database
- MongoDB (via config/db.js)

### AI Service
- Custom AI Engine (services/aiEngine.js)
- Used for quote comparison and decision support

## 📂 Project Structure

```
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