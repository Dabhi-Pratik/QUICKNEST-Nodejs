# 🏠 QUICKNEST - Full Stack Rental Property Platform

QUICKNEST is a modern full-stack rental property platform developed using **Node.js**, **Express.js**, and **MongoDB**.  
The project is designed to provide a smooth experience for users who want to explore, add, manage, and view rental properties online.

This project focuses on building a secure and scalable backend architecture with proper authentication, API structure, middleware handling, and database management.

---

# 📌 Project Overview

QUICKNEST helps users:

- Create and manage accounts
- Securely login using JWT authentication
- Add rental properties
- Update and delete properties
- Upload property images
- Browse available rental listings
- Manage property-related data efficiently

The application follows REST API architecture and uses MongoDB for storing user and property information.

---

# 🚀 Features

## 🔐 Authentication System

- User Registration
- User Login
- Password Hashing using bcryptjs
- JWT Token Authentication
- Protected Routes
- Authorization Middleware

---

## 🏡 Property Management

- Add New Property
- Edit Existing Property
- Delete Property
- View All Properties
- View Single Property Details
- Upload Property Images

---

## ⚙️ Backend Features

- RESTful API Structure
- MongoDB Database Integration
- Express Middleware
- Centralized Error Handling
- Environment Variable Support
- Clean Folder Structure
- Scalable Backend Architecture

---

# 🛠️ Technologies Used

| Technology | Description |
|------------|-------------|
| Node.js | JavaScript Runtime Environment |
| Express.js | Backend Framework |
| MongoDB | NoSQL Database |
| Mongoose | MongoDB ODM |
| JWT | Authentication & Authorization |
| bcryptjs | Password Encryption |
| Multer | File Upload Handling |
| dotenv | Environment Variables |
| Nodemon | Auto Restart Development Server |

---

# 📂 Project Folder Structure

```bash
QUICKNEST-Nodejs/
│
├── config/
│   └── db.js
│
├── controller/
│   ├── authController.js
│   ├── propertyController.js
│   └── userController.js
│
├── middleware/
│   ├── auth.js
│   ├── errorMiddleware.js
│   └── uploadMiddleware.js
│
├── models/
│   ├── userModel.js
│   └── propertyModel.js
│
├── routes/
│   ├── authRoutes.js
│   ├── propertyRoutes.js
│   └── userRoutes.js
│
├── uploads/
│
├── public/
│
├── views/
│
├── screenshots/
│
├── .env
├── .gitignore
├── app.js
├── package.json
└── README.md
```

---

# ⚙️ Installation Guide

Follow these steps to run the project locally on your system.

---

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/Dabhi-Pratik/QUICKNEST-Nodejs.git
```

---

## 2️⃣ Navigate to the Project Folder

```bash
cd QUICKNEST-Nodejs
```

---

## 3️⃣ Install Dependencies

```bash
npm install
```

This command installs all required npm packages used in the project.

---

## 4️⃣ Create Environment Variables

Create a `.env` file in the root directory and add the following:

```env
PORT=5000

MONGO_URI=your_mongodb_connection_string

JWT_SECRET=your_jwt_secret_key
```

### 🔍 Explanation

| Variable | Description |
|----------|-------------|
| PORT | Server running port |
| MONGO_URI | MongoDB database connection string |
| JWT_SECRET | Secret key used for JWT token generation |

---

## 5️⃣ Start Development Server

```bash
npm run dev
```

If everything is configured correctly, the server will start successfully.

---

# 🔐 Authentication Flow

QUICKNEST uses **JWT (JSON Web Token)** for secure authentication.

### Login Process

1. User logs in with email and password
2. Server verifies credentials
3. JWT token is generated
4. Token is returned to the client
5. Client sends token in Authorization header

---

## 🔑 Authorization Header Example

```bash
Authorization: Bearer YOUR_JWT_TOKEN
```

---

# 📮 API Endpoints

# 🔑 Authentication APIs

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/auth/register | Register New User |
| POST | /api/auth/login | Login User |

---

# 🏡 Property APIs

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/property | Get All Properties |
| GET | /api/property/:id | Get Single Property |
| POST | /api/property | Add New Property |
| PATCH | /api/property/:id | Update Property |
| DELETE | /api/property/:id | Delete Property |

---

# 🧪 API Request Examples

## 🔹 Register User

### Request Body

```json
{
  "name": "Pratik Dabhi",
  "email": "pratik@gmail.com",
  "password": "123456"
}
```

---

## 🔹 Login User

### Request Body

```json
{
  "email": "pratik@gmail.com",
  "password": "123456"
}
```

---

## 🔹 Add Property

### Request Body

```json
{
  "title": "Luxury Apartment",
  "location": "Ahmedabad",
  "price": 15000,
  "description": "Fully furnished apartment with modern facilities"
}
```

---

# 📸 Postman API Testing

All APIs of QUICKNEST were tested using Postman.

# User Apis

# Admin Apis

# Booking Apis

# Provider Apis

<img width="1920" height="1032" alt="Screenshot 2026-05-14 121937" src="https://github.com/user-attachments/assets/ae1d1506-7bd9-4bda-ae5c-4b9328a5c9a3" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 120659" src="https://github.com/user-attachments/assets/17c5feac-7150-4fa5-b9f6-d4c997fac11c" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 120547" src="https://github.com/user-attachments/assets/a0327b0c-947d-43a7-b128-c36b1abc344f" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 120506" src="https://github.com/user-attachments/assets/8c508130-4aee-42b2-855d-d6bbb81a832f" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 120354" src="https://github.com/user-attachments/assets/dd1e19f5-44e2-4409-9b2e-750d7829896f" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 113629" src="https://github.com/user-attachments/assets/0010ca0d-f650-4ea4-8c4f-b298ec321951" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 113503" src="https://github.com/user-attachments/assets/59bd7d66-0008-4d79-9f9c-f8447851dcb9" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 113417" src="https://github.com/user-attachments/assets/64956215-ef0b-4b9e-9c02-da689df6161c" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 113320" src="https://github.com/user-attachments/assets/c5f06d7f-19d0-4a9b-8d87-e65303a62b70" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 113201" src="https://github.com/user-attachments/assets/5b8315a4-be32-4751-991c-d631b7616ca2" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 112141" src="https://github.com/user-attachments/assets/71f90799-93f4-4e23-b52e-4017051bdabf" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 112046" src="https://github.com/user-attachments/assets/80bce9b9-28a7-46ab-9179-033b25050032" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 111842" src="https://github.com/user-attachments/assets/e90d716b-1266-4392-8785-9a35d84f87c9" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 111702" src="https://github.com/user-attachments/assets/9ac861ff-b3fa-43f1-bcad-0a1763c886d6" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 111436" src="https://github.com/user-attachments/assets/269471aa-b897-4ef2-90fd-d672c959075f" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 111402" src="https://github.com/user-attachments/assets/3d6c6149-ba42-479b-9133-cd862f96cd32" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 110738" src="https://github.com/user-attachments/assets/9c80f535-c7d7-49e8-beb5-c9f51d648968" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 110708" src="https://github.com/user-attachments/assets/013650fe-708a-4e5d-8529-47d00ad5087f" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 110547" src="https://github.com/user-attachments/assets/42dbe88d-08f3-443c-8c1b-a21d62a05efe" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 110241" src="https://github.com/user-attachments/assets/ce01a887-5b0c-4e75-af26-971c3847f618" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 110115" src="https://github.com/user-attachments/assets/d2797b5f-ce0c-40c7-847c-0a3a5fa716e8" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 105719" src="https://github.com/user-attachments/assets/2e205d75-6d94-48ed-b6d2-4327857b998e" />
<img width="1920" height="1032" alt="Screenshot 2026-05-14 122134" src="https://github.com/user-attachments/assets/70d351c6-2b3c-4af6-afce-0e6b28d57b70" />



# ❌ Error Handling

The project includes centralized error handling middleware to manage:

- Invalid API Routes
- Unauthorized Access
- JWT Verification Errors
- Validation Errors
- Database Errors
- Server Errors

This helps improve debugging and provides cleaner API responses.

---

# 🔥 Future Improvements

Some features planned for future updates:

- Property Booking System
- Admin Dashboard
- Wishlist Functionality
- Search & Filter System
- Google Maps Integration
- Payment Gateway Integration
- Reviews & Ratings
- Email Notifications
- Real-Time Chat

---

# 🌐 Deployment Platforms

This project can be deployed on:

- Render
- Railway
- Vercel
- Cyclic
- Heroku

---

# 📚 Learning Objectives

This project helps developers learn:

- Backend Development with Node.js
- REST API Development
- MongoDB Database Management
- Authentication & Authorization
- Middleware Handling
- File Uploading
- Error Handling
- Project Structure Best Practices

---

# 👨‍💻 Author

## Pratik Dabhi

### 🔗 GitHub
https://github.com/Dabhi-Pratik


---

# ⭐ Support

If you found this project useful, please give it a ⭐ on GitHub.  
It motivates and supports future development.

---

# 📜 License

This project is licensed under the MIT License.



