# CRUD API with Express and MongoDB Atlas

This project is a simple CRUD (Create, Read, Update, Delete) API for managing products, built using Express.js and MongoDB Atlas.

## Prerequisites

Before you begin, ensure you have the following installed on your local machine:

- [Node.js](https://nodejs.org/) (v12.x or later)
- npm (comes with Node.js)
- [MongoDB Atlas account](https://www.mongodb.com/cloud/atlas)

## Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name 
```
### 2. Install Dependencies
```bash
npm install
```

### 3. Set up environment variables

Create a .env file in the root of the project and add your MongoDB Atlas connection string:
```bash
MONGODB_URI=your-mongodb-atlas-connection-string
PORT=3000
```

### 4. Start the server
```bash
npm start
```

The server will start on http://localhost:3000.

API Endpoints

### Create a new product

URL: /products

Method: POST
Body:
{
  "name": "Product Name",
  "quantity": 10,
  "price": 100,
  "image": "http://example.com/image.png"
}

Get all products
URL: /products
Method: GET

Get a single product
URL: /products/:id
Method: GET

Update a product
URL: /products/:id
Method: PUT
Body:
{
  "name": "Updated Name",
  "quantity": 15,
  "price": 120,
  "image": "http://example.com/updated-image.png"
}


Delete a product
URL: /products/:id
Method: DELETE