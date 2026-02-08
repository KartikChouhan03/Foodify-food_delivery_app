# Foodify Admin Panel 🛡️

The **Foodify Admin Panel** is a dedicated interface for restaurant owners/administrators to manage the food catalog and process customer orders. Built with React and integrated with the main Foodify backend.

## ⚡ Features

### 1. Add Items

- Upload new food items to the menu.
- fields for:
  - **Image Upload**: Visually display the food item.
  - **Product Name**: Name of the dish.
  - **Description**: Details about ingredients or taste.
  - **Category**: Classify items (e.g., Salad, Rolls, Deserts).
  - **Price**: Set the cost.

### 2. List Items

- View a comprehensive table of all food items currently in the database.
- **Delete Functionality**: Remove items that are no longer available.

### 3. Orders Management

- 🛑 **Real-time Order Updates**: View incoming orders.
- **Order Details**: See items ordered, customer address, and total amount.
- **Status Updates**: Change the status of an order to keep the customer informed:
  - _Food Processing_
  - _Out for Delivery_
  - _Delivered_

## 🛠️ Tech Stack

- **React.js**: UI Library.
- **React Router Dom**: For routing between Add, List, and Order pages.
- **Axios**: For API communication.
- **React Toastify**: For notification popups (success/error messages).
- **CSS**: Custom styling for a clean, professional look.

## 🚀 Setup & Installation

1. **Install Dependencies**
   Ensure you are in the `admin` directory:

   ```bash
   cd admin
   npm install
   ```

2. **Run Development Server**
   ```bash
   npm run dev
   ```
   The admin panel will typically run on `http://localhost:5174` (or the next available port after the frontend).

## 🔗 Connection to Backend

The admin panel communicates with the backend server (typically running on port 4000). Ensure the backend is running for the admin panel to function correctly.

- **API URL**: Configured via `VITE_API_URL` environment variable or defaults to identifying the local backend.

---

Part of the **Foodify** project.
