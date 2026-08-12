# 🛒 MERN E-Commerce Application

A full-stack **MERN Stack E-Commerce application** designed to provide a complete online shopping experience with user authentication, product management, order processing, and secure payment integration.

## 🚀 Features

* 🔐 User authentication and authorization
* 👤 User management
* 🛍️ Product management
* 📦 Order management
* 💳 Stripe payment integration
* 🔑 JWT-based authentication
* 🔒 Password hashing with bcrypt
* 📧 Email integration using Nodemailer
* 🗄️ MongoDB database integration
* 🌐 RESTful API architecture
* ⚡ Express.js backend

## 🛠️ Tech Stack

### Frontend

* React.js
* HTML
* CSS
* JavaScript

### Backend

* Node.js
* Express.js

### Database

* MongoDB
* Mongoose

### Authentication & Security

* JSON Web Tokens (JWT)
* bcryptjs

### Payments

* Stripe

### Email

* Nodemailer

### Development Tools

* Nodemon
* Jest
* Git
* GitHub

## 📂 Project Structure

```text
mern-ecommerce/
│
├── client/
│   ├── public/
│   ├── src/
│   └── package.json
│
├── routes/
│   ├── auth.js
│   ├── products.js
│   ├── orders.js
│   └── users.js
│
├── models/
├── controllers/
├── middleware/
│
├── server.js
├── package.json
├── .env.example
├── .gitignore
└── README.md
```

> The exact folder structure may vary depending on the current implementation of the project.

## 🔌 API Routes

The backend exposes REST API routes for the main application modules:

| Module         | Endpoint        |
| -------------- | --------------- |
| Authentication | `/api/auth`     |
| Products       | `/api/products` |
| Orders         | `/api/orders`   |
| Users          | `/api/users`    |

These routes are configured in the Express server.

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/krishnamnamithaa/mern-ecommerce.git
```

### 2. Navigate to the project

```bash
cd mern-ecommerce
```

### 3. Install backend dependencies

```bash
npm install
```

### 4. Configure environment variables

Create a `.env` file in the backend root directory.

```env
NODE_ENV=development
PORT=5000

MONGODB_URI=mongodb://localhost:27017/ecommerce

JWT_SECRET=your_jwt_secret_here

STRIPE_SECRET_KEY=your_stripe_secret_key_here

EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_email_password

CLIENT_URL=http://localhost:3000
```

**Never commit your `.env` file to GitHub.**

### 5. Start the backend

For development:

```bash
npm run dev
```

For production:

```bash
npm start
```

## 🗄️ Database

The application uses **MongoDB** with **Mongoose** for database management.

The default local database configured for development is:

```text
mongodb://localhost:27017/ecommerce
```

You can replace this with a MongoDB Atlas connection string through the `MONGODB_URI` environment variable.

## 💳 Payment Integration

The application includes **Stripe** integration for payment processing.

The Stripe secret key should be stored securely in the `.env` file:

```env
STRIPE_SECRET_KEY=your_stripe_secret_key_here
```

Never expose your Stripe secret key in frontend code or commit it to GitHub.

## 📧 Email Integration

Email functionality is configured using **Nodemailer**.

Required environment variables include:

```env
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_email_password
```

## 🔐 Security

The application uses:

* JWT for authentication
* bcryptjs for password hashing
* Environment variables for sensitive configuration
* CORS for cross-origin requests

## 🧪 Testing

Run the available tests using:

```bash
npm test
```

## 🌐 Server

The backend runs on:

```text
http://localhost:5000
```

The root endpoint can be used to verify that the API is running:

```text
GET /
```

Expected response:

```json
{
  "message": "MERN E-Commerce API is running!"
}
```

## 📈 Future Improvements

* Product search and filtering
* Shopping cart enhancements
* Product reviews and ratings
* Admin dashboard
* Order tracking
* Wishlist functionality
* Improved payment workflow
* Cloud deployment
* Automated CI/CD pipeline

## 👩‍💻 Author

**Krishnam Namithaa**

Computer Science Engineering
VIT-AP University

### GitHub

https://github.com/krishnamnamithaa

---

⭐ If you find this project useful, consider giving it a star!
