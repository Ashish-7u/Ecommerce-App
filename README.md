# MERN Ecommerce 2024

A full-stack ecommerce web application built with the MERN stack (MongoDB, Express, React, Node.js).  
This project supports user authentication, product management, shopping cart, order processing, admin dashboard, and more.

---

## Features

### User Features
- User registration and login
- Browse products with filtering and sorting
- Product details with reviews
- Add to cart, update quantity, remove items
- Checkout with address management and PayPal payment
- View order history and order details

### Admin Features
- Admin authentication
- Add, edit, delete products
- Manage orders and update order status
- View dashboard analytics

---

## Project Structure

```
mern-ecommerce-2024/
│
├── client/         # React frontend (Vite, Redux Toolkit, TailwindCSS)
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── store/
│   │   ├── config/
│   │   └── ...
│   ├── public/
│   ├── package.json
│   └── ...
│
├── server/         # Express backend (Node.js, MongoDB, Mongoose)
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── helpers/
│   ├── server.js
│   └── ...
│
├── README.md
└── ...
```

---

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- MongoDB (local or Atlas)
- npm

---

### 1. Clone the Repository

```sh
git clone https://github.com/<your-username>/mern-ecommerce-2024.git
cd mern-ecommerce-2024
```

---

### 2. Setup the Server

```sh
cd server
npm install
```

- Create a `.env` file in the `server/` directory for environment variables (MongoDB URI, etc).

#### Example `.env`:
```
MONGODB_URI=mongodb://localhost:27017/mern-ecommerce
CLIENT_SECRET_KEY=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

- Start the server:
```sh
npm run dev
```
Server runs on [http://localhost:5000](http://localhost:5000)

---

### 3. Setup the Client

```sh
cd ../client
npm install
```

- Start the client:
```sh
npm run dev
```
Client runs on [http://localhost:5173](http://localhost:5173)

---

## Usage

- Visit [http://localhost:5173](http://localhost:5173) in your browser.
- Register a new user or login as admin.
- Explore products, add to cart, checkout, and manage orders.
- Admin can manage products and orders from the dashboard.

---

## Technologies Used

- **Frontend:** React, Redux Toolkit, Vite, TailwindCSS, Radix UI
- **Backend:** Node.js, Express, MongoDB, Mongoose, JWT, Cloudinary
- **Payments:** PayPal integration

---

## Folder Highlights

- `client/src/components`: UI components for shop and admin
- `client/src/pages`: Page-level components (Home, Listing, Checkout, etc.)
- `client/src/store`: Redux slices for state management
- `server/controllers`: Express route controllers
- `server/models`: Mongoose models (User, Product, Cart, Order, etc.)
- `server/routes`: Express route definitions

---
