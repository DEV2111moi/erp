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

---

## 🧠 AI Engine Highlights

- 📊 Groups quotes by product  
- ⚖️ Normalizes values (0 → 1 scale)  
- 🧮 Applies weighted scoring  
- 🥇 Ranks vendors automatically  

---

## 📌 Example Use Case

> You need to buy 100 keyboards.

| Vendor | Price | Delivery | Rating |
|--------|------|---------|--------|
| A      | ₹2000 | 3 days  | ⭐⭐⭐⭐⭐ |
| B      | ₹1800 | 7 days  | ⭐⭐⭐⭐  |
| C      | ₹2200 | 2 days  | ⭐⭐⭐   |

👉 AI instantly calculates and selects the **best overall deal**.


---

## 🧠 AI Evaluation Dashboard

Smartly analyzes and ranks vendor quotes using price, delivery time, and vendor rating.

- 🏆 Automatically identifies the **best vendor**
- 📊 Displays **detailed score breakdown**
- ⚡ Enables **quick, data-driven decisions**

---
<img width="2795" height="1548" alt="image" src="https://github.com/user-attachments/assets/630e5d21-ba1f-4413-a376-d2aff64c92f9" />
<br>
---
<img width="2793" height="1557" alt="image" src="https://github.com/user-attachments/assets/73cf3ad6-b12c-4079-a51c-08683dfd659e" /> <br>
---
<img width="2793" height="1545" alt="image" src="https://github.com/user-attachments/assets/ae188314-6324-4733-86ba-c6dffd858c64" />

