# Canine Academy 🐶

## Overview
Canine Academy is an **online dog training platform** designed to help dog owners train their pets conveniently from home. Our **subscription-based training plans** ensure personalized training based on the dog's needs. Additionally, we provide an **e-commerce store** for pet products, making it a one-stop solution for dog owners.

## Features 🚀
- 📌 **Personalized Dog Training Plans** – Different subscription tiers for tailored training.
- 🛒 **E-Commerce Store** – Buy pet products and training accessories.
- 🔐 **Secure Authentication** – JWT-based authentication for user security.
- 🔄 **State Management** – Implemented using Redux.
- 📡 **REST API** – Backend services for authentication, training plans, and store functionality.
- 🛠 **MERN Stack** – Fully developed using MongoDB, Express.js, React.js, and Node.js.

---

## Tech Stack 🛠️
### **Frontend:**
- React.js
- Redux Toolkit (API Slice for state management)
- Tailwind CSS (for styling)

### **Backend:**
- Node.js
- Express.js
- MongoDB (Mongoose for database modeling)
- JWT Authentication

### **Other Tools & Libraries:**
- Axios (for API requests)
- bcrypt.js (for password hashing)
- Multer (for handling file uploads)
- dotenv (for environment variables)

---

## Installation & Setup 🏗️
### **1. Clone the Repository**
```sh
git clone https://github.com/your-username/canine-academy.git
cd canine-academy
```

### **2. Backend Setup**
```sh
cd backend
npm install
```
#### **Environment Variables**
Create a `.env` file in the `backend` folder and add:
```sh
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```
Run the backend server:
```sh
npm start
```

### **3. Frontend Setup**
```sh
cd ../frontend
npm install
npm start
```

The application will be live at `http://localhost:3000/` 🚀

---

## Folder Structure 📂
```
canine-academy/
 ├── backend/
 │   ├── models/        # Mongoose Models (User, TrainingPlan, Product, etc.)
 │   ├── routes/        # Express API Routes
 │   ├── controllers/   # Controller functions
 │   ├── middleware/    # Authentication & Error Handling Middleware
 │   ├── config/        # Database Configuration
 │   ├── server.js      # Main Express Server File
 │   ├── .env           # Environment Variables
 │
 ├── frontend/
 │   ├── src/
 │   │   ├── components/   # Reusable React Components
 │   │   ├── app/          # Redux Store (API Slice, Reducers, etc.)
 │   │   ├── features/     # All the features of the web app
 │   │   ├── images/       # images used in the frontend
 │   │   ├── App.js        # Main App File
 │   │   ├── index.js      # React Entry Point
 │
 ├── README.md        # Project Documentation
 ├── package.json     # Dependencies & Scripts
 ├── .gitignore       # Ignored Files
```

---

## API Endpoints 📡
### **Authentication**
- `POST /api/users/register` – Register a new user
- `POST /api/users/login` – Login and get a token
- `GET /api/users/profile` – Get user profile (requires authentication)

### **Dog Training Plans**
- `GET /api/training` – Get all training plans
- `POST /api/training` – Create a new training plan (Admin only)
- `PUT /api/training/:id` – Update training plan (Admin only)
- `DELETE /api/training/:id` – Delete training plan (Admin only)

### **E-Commerce Store**
- `GET /api/products` – Get all products
- `GET /api/products/:id` – Get product details
- `POST /api/orders` – Place an order

---

## Contributing 🤝
Want to contribute? Follow these steps:
1. Fork the repository 📌
2. Create a new feature branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -m 'Added new feature'`)
4. Push to the branch (`git push origin feature-name`)
5. Open a Pull Request ✨

---

## License 📜
This project is licensed under the **MIT License**.

---

## Contact & Support 📧
For any issues or suggestions, feel free to open an issue or contact us at **your-email@example.com**.

📢 *Train your dog easily & shop for pet products with Canine Academy!* 🐾
