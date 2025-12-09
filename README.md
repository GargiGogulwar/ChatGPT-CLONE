# 🌟 ChatGPT-CLONE

A fully customizable clone of ChatGPT built using **React (Vite)**, **Node.js**, **Express**, **MongoDB**, and **OpenAI API**.  
Supports **user authentication**, **email verification**, **JWT-based login**, and a beautiful chat UI similar to ChatGPT.

---

# 🚀 Features

## 🔐 Authentication & Security
- User **sign-up + login**
- Email verification via **Gmail SMTP**
- Password hashing (**bcrypt**)
- JWT authentication for protected routes

## 💬 AI Chatbot
- Chat interface similar to ChatGPT
- Uses OpenAI’s API (customizable model)
- Backend proxy for secure API calls

## 📦 Backend (Node + Express)
- REST API endpoints
- MongoDB using Mongoose
- MVC structure (Routes + Controllers)
- Environment-based config

## 🎨 Frontend (React + Vite)
- Modern, fast UI
- Tailwind CSS styling
- Axios API service
- Chat bubbles & clean UI components

## 📧 Email System
- SMTP using Gmail
- Sends verification emails
- MAIL_EMAIL + MAIL_SECRET configurable

## 🗄 Database (MongoDB)
- Stores users
- Stores verification status
- (Optional) chat history

---

# 🛠 Tech Stack

### **Frontend**
- React (Vite)
- Tailwind CSS
- Axios

### **Backend**
- Node.js  
- Express.js  
- Mongoose  
- JWT  
- Nodemailer  

### **AI**
- OpenAI API (gpt-3.5-turbo-instruct or newer)

---

# 📁 Folder Structure

ChatGPT-CLONE/
│
├── client/ # Frontend (React + Vite)
│ ├── src/
│ ├── public/
│ └── .env.local
│
├── server/ # Backend (Node + Express)
│ ├── routes/
│ ├── controllers/
│ ├── models/
│ ├── db/
│ └── .env
│
└── README.md


---

# ⚙️ Environment Variables

## 🟦 Backend (`server/.env`)
```env
PORT=5000
MONGO_URL=mongodb://127.0.0.1:27017/chatgpt
SITE_URL=http://localhost:5173
JWT_PRIVATE_KEY=your_jwt_secret
OPENAI_API_KEY=your_openai_key
OPENAI_ORGANIZATION=
MAIL_EMAIL=your_gmail_account
MAIL_SECRET=your_app_password
🟩 Frontend (client/.env.local)
VITE_CLIENT_ID=your_google_oauth_id
```
🧩 How to Run the Project Locally
1️⃣ Clone the Repository
git clone https://github.com/GargiGogulwar/ChatGPT-CLONE.git

2️⃣ Install Backend Dependencies
cd server
npm install
npm start

3️⃣ Install Frontend Dependencies
cd ../client
npm install
npm run dev

4️⃣ Open the App

👉 http://localhost:5173

🔑 API Keys & Setup
✔ OpenAI API Key

Create one from:
https://platform.openai.com/settings/keys

✔ Gmail App Password

Steps:

Google Account

Security → App Passwords

Create 16-digit password

Use as MAIL_SECRET

🧪 Troubleshooting
❌ Chat not responding?

Check backend console

Ensure correct model (gpt-3.5-turbo-instruct)

Make sure your OpenAI account has credit

❌ Email not sending?

Use Gmail App Password, not normal password

Ensure less secure app access is allowed

❌ Backend returning 500?

Wrong OpenAI API key

Incorrect model

Problem with env variables

✨ Author

Gargi Gogulwar
