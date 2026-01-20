# 🛒 Secure E-Com

Secure E-Com is a **full-stack e-commerce web application** built with the **MERN stack (MongoDB, Express.js, React.js, Node.js)**.  
It provides a secure platform for users to browse products, manage a shopping cart, and place orders, while enabling admins to manage the product catalog.

---

## ✨ Features

- 🔐 **User Authentication** – Signup, login, and JWT-based authorization  
- 📦 **Product Catalog** – Browse, search, and view detailed product pages  
- 🛍️ **Shopping Cart** – Add, update, and remove items from the cart  
- 💳 **Order Management** – Simulated checkout and order history tracking  
- ⚙️ **Admin Panel** – CRUD operations (Create, Read, Update, Delete) for products  
- 📱 **Responsive UI** – Built with React.js for desktop and mobile devices  
- 🛡 **Security** – Password hashing, protected routes, and token validation  

---

## 🛠 Tech Stack

- **Frontend:** React.js, HTML, CSS, JavaScript  
- **Backend:** Node.js, Express.js (REST APIs)  
- **Database:** MongoDB (NoSQL)  
- **Authentication:** JSON Web Tokens (JWT), bcrypt  
- **Tools & Other:** Git, npm, Concurrently, Postman for API testing  

---

## 📂 Project Structure

```
mern-ecommerce-master_2/
├── backend/              # Node/Express server
│   ├── models/           # Mongoose schemas (User, Product, Order)
│   ├── routes/           # API routes
│   ├── controllers/      # Business logic
│   ├── middleware/       # Authentication, error handling
│   └── server.js         # Entry point
│
├── frontend/             # React.js frontend
│   ├── src/
│   │   ├── components/   # UI components
│   │   ├── pages/        # Screens (Home, Product, Cart, Login, Admin)
│   │   ├── services/     # API calls
│   │   └── App.js
│   └── public/
│
├── package.json          # Dependencies
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/Reethureddie/Secure-ecom-mern.git
cd Secure-ecom-mern/mern-ecommerce-master_2
```

### 2. Backend setup
```bash
cd backend
npm install
cp .env.example .env     # Add MongoDB URI, JWT_SECRET, PORT
npm run dev
```

### 3. Frontend setup
```bash
cd frontend
npm install
npm start
```

### 4. Access
- Frontend → http://localhost:3000  
- Backend API → http://localhost:5000/api/...

---

## 📋 API Endpoints

| Endpoint            | Method | Description             |
|---------------------|--------|-------------------------|
| /api/auth/signup    | POST   | Register a new user     |
| /api/auth/login     | POST   | Authenticate user (JWT) |
| /api/products       | GET    | Fetch all products      |
| /api/products/:id   | GET    | Fetch product by ID     |
| /api/products       | POST   | Add product (admin only)|
| /api/products/:id   | PUT    | Update product (admin)  |
| /api/products/:id   | DELETE | Delete product (admin)  |
| /api/cart           | POST   | Add item to cart        |
| /api/orders         | GET    | View user orders        |

---

## 🧪 Testing

- APIs tested with Postman  
- Basic validation for inputs and JWT tokens  
- Run unit tests (if added): `npm test`  

---

## 🌱 Future Enhancements

- Add Stripe/PayPal payment integration  
- Role-based access (admin vs user)  
- Product image uploads with Cloudinary/AWS S3  
- Improve mobile UI responsiveness  
- Add automated tests with Jest/Mocha  

---

## 📄 License

This project is licensed under the MIT License – free to use and modify.

---

## 👩‍💻 Author

Developed by **Reethika Reddy Danda** – [GitHub](https://github.com/Reethureddie)
