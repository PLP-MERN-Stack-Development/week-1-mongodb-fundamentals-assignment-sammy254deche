[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=19673379&assignment_repo_type=AssignmentRepo)
# MongoDB Fundamentals Assignment

This assignment focuses on learning MongoDB fundamentals including setup, CRUD operations, advanced queries, aggregation pipelines, and indexing.

## Assignment Overview

You will:
1. Set up a MongoDB database
2. Perform basic CRUD operations
3. Write advanced queries with filtering, projection, and sorting
4. Create aggregation pipelines for data analysis
5. Implement indexing for performance optimization

## Getting Started

1. Accept the GitHub Classroom assignment invitation
2. Clone your personal repository that was created by GitHub Classroom
3. Install MongoDB locally or set up a MongoDB Atlas account
4. Run the provided `insert_books.js` script to populate your database
5. Complete the tasks in the assignment document

## Files Included

- `Week1-Assignment.md`: Detailed assignment instructions
- `insert_books.js`: Script to populate your MongoDB database with sample book data

## Requirements

- Node.js (v18 or higher)
- MongoDB (local installation or Atlas account)
- MongoDB Shell (mongosh) or MongoDB Compass

## Submission

Your work will be automatically submitted when you push to your GitHub Classroom repository. Make sure to:

1. Complete all tasks in the assignment
2. Add your `queries.js` file with all required MongoDB queries
3. Include a screenshot of your MongoDB database
4. Update the README.md with your specific setup instructions

## Resources

- [MongoDB Documentation](https://docs.mongodb.com/)
- [MongoDB University](https://university.mongodb.com/)
- [MongoDB Node.js Driver](https://mongodb.github.io/node-mongodb-native/) 



🛍️ Product Management API
A RESTful API built with Express.js and MongoDB for managing products. This project is part of the Week 2 Express.js Assignment for the PLP Program.

🚀 Features
CRUD operations for products
Middleware for logging, validation, and authentication
MongoDB integration using Mongoose
Pagination, filtering, and search
Product statistics by category
Error handling and custom error classes
🧾 Tech Stack
Node.js
Express.js
MongoDB & Mongoose
Postman (for API testing)
📦 Installation & Setup
Clone the repository:
git clone https://github.com/PLP-MERN-Stack-Development/week-2-express-js-assignment-Samuel.git
cd product-api
Install dependencies:

bash
Copy code
pnpm install
Start MongoDB (locally or using a MongoDB Atlas URI).

Run the server:

bash
Copy code
pnpm run dev
Server will start on: http://localhost:3000

🔐 Authentication
All requests must include a valid API key in the headers:

vbnet
Copy code
x-api-key: my-secret-key
You can change the key in middleware/auth.js or via .env.

📘 API Endpoints
📍 Base URL
bash
Copy code
/api/products
➕ POST /
Create a new product

📥 GET /
Get all products with optional query parameters:

category: filter by category

inStock: true or false

page: page number (default: 1)

limit: items per page (default: 5)

🔍 GET /search?name=keyword
Search products by name (case-insensitive)

📊 GET /stats
Get stats grouped by category:

total count

average price

number in stock

🆔 GET /:id
Get a product by ID

✏️ PUT /:id
Update a product by ID

❌ DELETE /:id
Delete a product by ID

📁 Folder Structure
pgsql
Copy code
.
├── middleware/
│   ├── auth.js
│   ├── logger.js
│   ├── validateProduct.js
│   └── errorHandler.js
├── routes/
│   └── products.js
├── utils/
│   └── errors.js
├── Products.js
├── server.js
├── package.json
└── README.md
📬 Example Request
http
Copy code
POST /api/products
x-api-key: my-secret-key
Content-Type: application/json

{
  "name": "Wireless Mouse",
  "description": "Ergonomic design",
  "price": 25,
  "category": "accessories",
  "inStock": true
}


🧑‍💻 Author
Samuel Deche 
MERN Stack Developer | PLP Participant





MongoDB Fundamentals Assignment
Author: Samuel
This project demonstrates the use of MongoDB for data insertion, querying, aggregation, and indexing using the MongoDB shell and Compass.

📁 Files Included:
insert_books.js – Script to insert 10+ book documents.
queries.js – MongoDB queries for CRUD, advanced operations, and aggregation.
Screenshot(s) – Showing the inserted data in MongoDB Compass.
🧪 How to Run
Start MongoDB locally or connect to MongoDB Atlas.

Insert the books:

mongosh < insert_books.js
Open MongoDB Shell (mongosh) or Compass Shell, then run queries from queries.js.

📸 Screenshot Screenshots are in the screenshots/ folder, showing:

The books collection with inserted data.