# 🛡️ Auth System (Node.js, Express, MongoDB)

A simple and secure authentication system with features like user registration, login, password reset (via code), JWT-based session handling, and protected routes for dashboard access.

## 🚀 Features

- User Registration
- Secure Login with JWT Authentication
- Password Reset via Email Code (simplified logic)
- Protected Dashboard Route
- Frontend: HTML, CSS, Vanilla JS
- Backend: Node.js, Express.js, MongoDB
- Middleware for JWT protection

---

## 📁 Project Structure
auth_system/
├── controllers/
│ └── authController.js
├── middleware/
│ └── authMiddleware.js
├── models/
│ └── User.js
├── public/
│ ├── login.html
│ ├── register.html
│ ├── dashboard.html
│ └── style.css
├── routes/
│ └── authRoutes.js
├── .env
├── server.js
└── package.json

yaml
Copy
Edit

---

## 🔧 Installation

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/auth_system.git
cd auth_system
Install dependencies:

bash
Copy
Edit
npm install
Setup environment variables (.env):

env
Copy
Edit
PORT=5000
MONGO_URI=mongodb://localhost:27017/auth_system
JWT_SECRET=your_jwt_secret_key
Run the server:

bash
Copy
Edit
npm start
🌐 Frontend Pages
/public/login.html – Login Page

/public/register.html – Register Page

/public/dashboard.html – Protected User Dashboard

Open the HTML files in a browser (served statically via Express).

🔐 API Endpoints
Method	Route	Description	Access
POST	/api/auth/register	Register a new user	Public
POST	/api/auth/login	Authenticate user	Public
GET	/api/auth/dashboard	Get user info	Protected
POST	/api/auth/reset-request	Request password reset code	Public
POST	/api/auth/reset-password	Submit reset code and password	Public

🧪 Sample Test User
json
Copy
Edit
{
  "email": "student@example.com",
  "password": "securePassword123"
}
📌 Notes
This is a basic educational project — no actual email sending.

The reset code is stored in the DB temporarily and verified manually.

Tokens are stored in localStorage and attached to the Authorization header.

📸 Wireframes
Login & Dashboard wireframes included in /wireframes/ folder or generated via ChatGPT.

✅ To Do
Add real email service (Nodemailer)

Implement logout token blacklisting

Add user roles (admin/user)

Deploy on Render/Heroku/Vercel

🧑‍💻 Author
Made by [Your Name] – Contributions welcome!

📄 License
MIT License

yaml
Copy
Edit

---

Let me know if you want a **version with screenshots**,

