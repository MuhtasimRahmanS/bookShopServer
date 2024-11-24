# **Book Shop Application**

A **Express.js** application built with **TypeScript** to manage a book store, leveraging **MongoDB** for database operations and **Mongoose** for schema modeling. This application offers managing books and orders with efficient CRUD operations and data validation.

---

## **Features**

### **Books Management**

- **Create**: Add new books with details like title, author, price, category, description, and stock quantity.
- **Read**: Retrieve all books or filter by title, author, or category.
- **View Details**: Fetch detailed information for any specific book by its ID.
- **Update**: Modify book information, such as price, quantity, and stock status.
- **Delete**: Remove books from the database.

### **Orders Management**

- **Create Order**: Place orders for books with automatic stock adjustment.
- **Stock Validation**: Prevent orders if stock is insufficient.
- **Revenue Calculation**: Calculate total revenue using MongoDB's aggregation pipeline.

### **Error Handling**

- Detailed error messages with consistent structure.
- Input validation at all stages to ensure data integrity.

### **Performance Optimizations**

- Efficient database queries with indexed fields for faster search.
- Aggregate pipelines for complex computations (e.g., revenue calculations).

---

## **Technologies Used**

- **Backend Framework**: Express.js with TypeScript
- **Database**: MongoDB with Mongoose
- **Validation**: Zod and Mongoose schema validation
- **Development Tools**: ESLint, Prettier, Nodemon

---

## **API Endpoints**

## **Books**

- **Create a Book**: POST /api/products
- **Get All Books**: GET /api/products?searchTerm={term}
- **Get Book by ID**: GET /api/products/:productId
- **Update Book**: PUT /api/products/:productId
- **Delete Book**: DELETE /api/products/:productId

## **Orders**

- **Create Order**: POST /api/orders
- **Get Total Revenue**: GET /api/orders/revenue

---

## **Setup Instructions**

### **Prerequisites**

Make sure you have the following installed on your system:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
- [MongoDB](https://www.mongodb.com/) (local or cloud-based like [MongoDB Atlas](https://www.mongodb.com/cloud/atlas))

### **Step-by-Step Setup**

1. **Clone the Repository**

   ```bash
   git clone https://github.com/MuhtasimRahmanS/bookShopServer.git
   ```

1. **Install Dependencies**

   ```bash
   npm install
   ```

   or

   ```bash
   yarn install
   ```

1. **Run the Application**

   ```bash
   npm run dev
   ```
