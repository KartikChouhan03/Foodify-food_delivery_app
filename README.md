project:
  name: Foodify – Full Stack Food Delivery Web App
  description: >
    Foodify is a full-stack food delivery web application built using the MERN stack,
    featuring a customer-facing frontend, an admin dashboard, and a RESTful backend API.
    The project is deployed using modern cloud platforms and follows real-world deployment practices.

live_demo:
  frontend_user_app: https://food-delivery-frontend-tawny.vercel.app
  backend_api: https://foodify-food-delivery-app.onrender.com
  admin_panel: https://food-delivery-admin-lime.vercel.app/
  note: >
    The backend is hosted on Render (free tier) and may take 30–60 seconds to respond
    on the first request due to cold start.

tech_stack:
  frontend:
    - React.js
    - Vite
    - Axios
    - CSS / Tailwind (if applicable)
    - Deployed on Vercel
  backend:
    - Node.js
    - Express.js
    - MongoDB (Atlas)
    - JWT Authentication
    - REST API architecture
    - Deployed on Render
  database:
    - MongoDB Atlas (Free Tier)

core_features:
  user_features:
    - Browse food items
    - Add/remove items from cart
    - Place orders
    - View order summary
    - Authentication (JWT-based)
  admin_features:
    - Secure admin login
    - Add / update / delete food items
    - View orders
    - Manage food catalog
  backend_features:
    - RESTful API design
    - Secure JWT authentication
    - Environment-based configuration
    - Proper CORS handling
    - Cloud database integration

project_architecture:
  root: Foodify/
  structure:
    - frontend/: User-facing React app
    - admin/: Admin dashboard (React)
    - backend/:
        - routes/
        - models/
        - controllers/
        - index.js

environment_variables:
  backend_render:
    MONGO_URI: your_mongodb_atlas_connection_string
    JWT_SECRET: your_random_secret_key
  frontend_and_admin_vercel:
    VITE_API_URL: https://foodify-food-delivery-app.onrender.com

local_setup_optional:
  backend:
    steps:
      - cd backend
      - npm install
      - npm start
  frontend:
    steps:
      - cd frontend
      - npm install
      - npm run dev
  admin_panel:
    steps:
      - cd admin
      - npm install
      - npm run dev

key_learnings:
  - Real-world deployment of a full-stack MERN application
  - Handling environment variables across platforms
  - MongoDB Atlas configuration and IP whitelisting
  - CORS and cross-origin API communication
  - Cloud deployment limitations (cold starts, free tiers)
  - Separating frontend, backend, and admin concerns

notes:
  - This project was initially developed locally and later adapted for cloud deployment.
  - The backend may sleep when inactive due to Render’s free tier limitations.
  - MongoDB Atlas free clusters may auto-pause when idle.

author:
  name: Kartik Chouhan


GitHub: https://github.com/KartikChouhan03

📄 License

This project is for educational and learning purposes.
