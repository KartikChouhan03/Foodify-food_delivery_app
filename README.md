# Foodify 🍔

Foodify is a full-stack food delivery application that brings delicious meals right to your doorstep. Built with the MERN stack (MongoDB, Express, React, Node.js), it features a seamless ordering experience for users and a comprehensive admin panel for restaurant management.

## 🚀 Features

### User Frontend

- **Browse Menu**: Explore a wide variety of food items categorized for easy navigation.
- **Cart Management**: Add items to the cart, adjust quantities, and view the total cost.
- **Secure Checkout**: Place orders securely (integrated with Stripe/Razorpay).
- **Order Tracking**: View order status and history in "My Orders".
- **Authentication**: Secure login and registration system.
- **Responsive Design**: Optimized for both desktop and mobile devices.

### Admin Panel

- **Add Items**: Upload new food items with images, descriptions, prices, and categories.
- **List Items**: View all available food items and manage them (delete/edit).
- **Order Management**: View customer orders and update their status (e.g., Food Processing, Out for Delivery, Delivered).

## 🛠️ Tech Stack

### Frontend & Admin

- **React.js**: Library for building user interfaces.
- **Vite**: Next-generation frontend tooling.
- **React Router**: For navigation and client-side routing.
- **Axios**: For making HTTP requests to the backend.
- **CSS3 / CSS Modules**: For styling (with custom animations and responsive layouts).

### Backend

- **Node.js & Express.js**: Server-side runtime and framework.
- **MongoDB & Mongoose**: NoSQL database for flexible data storage.
- **JWT (JSON Web Tokens)**: For secure user authentication.
- **Bcrypt**: For password hashing.
- **Multer**: For handling image uploads.
- **Stripe / Razorpay**: Payment gateway integration.
- **Validator**: For input validation.

## 📂 Project Structure

- `frontend/`: React application for customers.
- `admin/`: React application for administrators.
- `backend/`: Node.js/Express API server.

## ⚙️ Installation & Setup

Follow these steps to set up the project locally.

### Prerequisites

- Node.js (v14+ recommended)
- MongoDB (Local or Atlas connection string)

### 1. Backend Setup

Navigate to the backend directory and install dependencies:

```bash
cd backend
npm install
```

Create a `.env` file in the `backend` directory with the following variables:

```env
PORT=4000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
```

Start the server:

```bash
npm run server
```

The server will run on `http://localhost:4000`.

### 2. Frontend Setup

Navigate to the frontend directory and install dependencies:

```bash
cd frontend
npm install
```

Start the development server:

```bash
npm run dev
```

The app will open at `http://localhost:5173`.

### 3. Admin Panel Setup

Navigate to the admin directory and install dependencies:

```bash
cd admin
npm install
```

Start the admin dashboard:

```bash
npm run dev
```

## 📡 API Endpoints

The backend exposes the following RESTful API endpoints:

| Method   | Endpoint                | Description                 |
| :------- | :---------------------- | :-------------------------- |
| **GET**  | `/api/food/list`        | Get all food items          |
| **POST** | `/api/food/add`         | Add a new food item (Admin) |
| **POST** | `/api/food/remove`      | Remove a food item (Admin)  |
| **POST** | `/api/user/register`    | Register a new user         |
| **POST** | `/api/user/login`       | User login                  |
| **POST** | `/api/cart/add`         | Add item to cart            |
| **POST** | `/api/cart/remove`      | Remove item from cart       |
| **POST** | `/api/cart/get`         | Get user cart               |
| **POST** | `/api/order/place`      | Place an order              |
| **POST** | `/api/order/userorders` | Get specific user orders    |
| **GET**  | `/api/order/list`       | List all orders (Admin)     |
| **POST** | `/api/order/status`     | Update order status (Admin) |

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

Developed with ❤️ by [Your Name]
