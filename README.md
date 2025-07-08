# 🌟 TheLuxora

TheLuxora is a full-stack e-commerce web application built with the MERN stack (MongoDB, Express, React, Node.js). It features user authentication, product management, shopping cart, coupon system, Stripe payments, analytics dashboard, and more.

## ✨ Features

- 🔐 **User Authentication:** Sign up, login, logout, JWT-based authentication with refresh tokens.
- 🛠️ **Admin Dashboard:** Create, delete, and manage products; view analytics.
- 🛍️ **Product Catalog:** Browse products by category, view featured products, and recommendations.
- 🛒 **Shopping Cart:** Add, remove, and update product quantities in the cart.
- 🎟️ **Coupons:** Apply and manage discount coupons.
- 💳 **Stripe Payments:** Secure checkout and order processing.
- 📦 **Order Management:** Track purchases and order history.
- 📊 **Analytics:** Visualize sales, revenue, and user statistics (admin only).
- 📱 **Responsive UI:** Modern, mobile-friendly design using Tailwind CSS and React.

## 🗂️ Project Structure

```
.
├── backend/
│   ├── controllers/
│   ├── lib/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   └── server.js
├── frontend/
│   ├── public/
│   ├── src/
│   ├── index.html
│   ├── package.json
│   └── ...
├── .env
├── package.json
└── README.md
```

## 🚀 Getting Started

### 🛠️ Prerequisites

- Node.js (v18+ recommended)
- npm
- MongoDB Atlas account (or local MongoDB)
- [Stripe](https://stripe.com/) account
- [Cloudinary](https://cloudinary.com/) account
- [Upstash Redis](https://upstash.com/) account

### ⚙️ Environment Variables

Create a `.env` file in the root directory with the following variables:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
UPSTASH_REDIS_URL=your_redis_url
ACCESS_TOKEN_SECRET=your_access_token_secret
REFRESH_TOKEN_SECRET=your_refresh_token_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
CLIENT_URL=http://localhost:5173
NODE_ENV=development
```

### 📦 Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/theluxora.git
   cd theluxora
   ```

2. **Install backend and frontend dependencies:**
   ```sh
   npm install
   cd frontend
   npm install
   cd ..
   ```

### 🏃 Running the Application

#### 🧑‍💻 Development

Start both backend and frontend (Vite) servers:

```sh
npm run dev
```

- Backend: [http://localhost:5000](http://localhost:5000)
- Frontend: [http://localhost:5173](http://localhost:5173)

#### 🏗️ Production Build

To build the frontend for production:

```sh
npm run build
```

This will install dependencies and build the frontend in `frontend/dist`.

To start the production server:

```sh
npm start
```

### 🔗 API Endpoints

- **Auth:** `/api/auth`
- **Products:** `/api/products`
- **Cart:** `/api/cart`
- **Coupons:** `/api/coupons`
- **Payments:** `/api/payments`
- **Analytics:** `/api/analytics` (admin only)

### 🛠️ Technologies Used

- **Backend:** Node.js, Express, MongoDB, Mongoose, JWT, Redis, Stripe, Cloudinary
- **Frontend:** React, Vite, Zustand, React Router, Tailwind CSS, Framer Motion, Stripe.js
- **Other:** ESLint, dotenv, nodemon

### 📁 Folder Overview

- `backend/`: Express server, API routes, controllers, models, middleware, and integrations.
- `frontend/`: React app, components, pages, Zustand stores, and static assets.

### 📝 Customization

- 👑 **Admin Access:** By default, users are created with the "customer" role. To make a user admin, manually update their role in the database.
- 💳 **Stripe & Cloudinary:** Replace the test keys in `.env` with your own for production.

### 📄 License

This project is licensed under the ISC License.

---

⚠️ **Note:** For security, never commit your `.env` file or sensitive credentials to version control.

---

## 👤 Author

- [Kumar Navin](https://github.com/Navin0062)