# Online Shop - E-Commerce Application

A full-featured e-commerce platform built with Node.js, Express, MongoDB, and EJS templates.

## 🛠 Tech Stack

- **Backend:** Node.js, Express
- **Database:** MongoDB (native driver)
- **Templating:** EJS
- **Authentication:** express-session + MongoDB session store
- **Security:** CSRF protection, bcryptjs password hashing
- **File Upload:** Multer
- **Dev Tools:** Nodemon (auto-restart)

## 🚀 Features

- User authentication (register/login)
- Product catalog with search & filtering
- Shopping cart management
- Order processing & history
- Admin panel for product/order management
- Image upload for products
- CSRF protection
- Session-based cart

- ## 📁 Project Structure

```
├── app.js                 # Main application entry point
├── config/                # Configuration files
│   └── session.js         # MongoDB session configuration
├── controllers/           # Route controllers (business logic)
│   ├── admin.controller.js
│   ├── auth.controller.js
│   ├── cart.controller.js
│   ├── orders.controller.js
│   └── products.controller.js
├── data/                  # Database connection
├── middlewares/           # Custom middleware functions
│   ├── cart.js            # Cart initialization
│   ├── check-auth.js      # Authentication check
│   ├── csrf-token.js      # CSRF token injection
│   ├── error-handler.js   # Global error handling
│   ├── image-upload.js    # Multer file upload handler
│   ├── not-found.js       # 404 handler
│   ├── protect-routes.js  # Route protection
│   └── update-cart-prices.js
├── models/                # MongoDB data models
│   ├── cart.models.js
│   ├── order.model.js
│   ├── product.model.js
│   └── user.model.js
├── product-data/          # Static product images
├── public/                # Public static assets (CSS, JS)
├── routes/                # Express route definitions
│   ├── admin.routes.js
│   ├── auth.routes.js
│   ├── base.routes.js
│   ├── cart.routes.js
│   ├── orders.routes.js
│   └── products.routes.js
├── util/                  # Utility functions
└── views/                 # EJS templates
    ├── admin/             # Admin panel views
    ├── customer/          # Customer-facing views
    └── shared/            # Partials (header, footer, etc.)
```

## 📦 Installation

```bash
npm install
```

## ▶️ Run

```bash
npm start
```

Server runs on `http://localhost:3000`

## 🔧 Environment Variables

Create a `.env` file with:
```
MONGODB_URI=mongodb://localhost:27017/shop
SESSION_SECRET=your_secret_key
```
