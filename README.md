# Inventory and Data Management System

A RESTful backend API built with Node.js, Express.js, and MongoDB to manage a store's product catalogue, stock levels, and inventory reports.

## 🚀 Features
- Complete CRUD operations for products
- Mongoose schema validation & virtual fields (`stockValue`)
- Query-string filtering, sorting, and pagination
- MongoDB Aggregation pipelines for Low-Stock Alerts and Category Summaries
- Centralized error handling middleware
- Secure environment variable management using `dotenv`

## 🛠️ Tech Stack
- **Runtime:** Node.js
- **Framework:** Express.js
- **Database:** MongoDB (Mongoose ODM)
- **Environment:** dotenv

## 📦 Installation & Setup
1. Clone the repository: `git clone <your-repo-url>`
2. Install dependencies: `npm install`
3. Create a `.env` file and add your `MONGO_URI` and `PORT=5000`
4. Start the server: `npm run dev`

## 📌 API Endpoints
- `POST /api/products` - Create a new product
- `GET /api/products` - Get all products (supports pagination, sorting, filtering)
- `GET /api/products/:id` - Get a single product
- `PUT /api/products/:id` - Update product details
- `PATCH /api/products/:id/stock` - Adjust stock levels safely
- `DELETE /api/products/:id` - Delete a product
- `GET /api/products/low-stock` - Get low-stock alert report
- `GET /api/products/summary` - Get category-wise inventory summary