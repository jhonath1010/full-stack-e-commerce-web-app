
# 🛒 Full-Stack E-Commerce Web App

A full-stack Node.js e-commerce application that supports user authentication, product and category management, and dynamic page rendering with EJS templates. The backend integrates both MongoDB and PostgreSQL for a hybrid data storage solution.

## 📋 Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Environment Variables](#environment-variables)
  - [Running the App](#running-the-app)
- [License](#license)

## 📖 About the Project

This application demonstrates a full-stack solution using Node.js and Express.js with dynamic EJS templates. It showcases a modular approach to authentication and e-commerce functionality by separating logic into `auth-service.js` and `store-service.js`.

## 🚀 Features

- User registration and login with password hashing using bcrypt
- Session management with express-session
- Product and category CRUD operations via PostgreSQL and Sequelize
- EJS-powered views for server-side rendering
- Static asset handling through a public folder

## 🛠 Tech Stack

### Backend
- Node.js
- Express.js
- PostgreSQL (via Sequelize ORM)
- MongoDB (via Mongoose ODM)
- bcrypt.js
- express-session

### Frontend
- EJS
- HTML/CSS
- Bootstrap, Tailwind CSS (optional)

## 🗂️ Project Structure

```
full-stack-e-commerce-web-app/
├── auth-service.js            # Handles authentication logic
├── store-service.js           # Manages products and categories
├── server.js                  # Main server entry point
├── views/                     # EJS templates
├── public/                    # Static assets (CSS, JS, images)
├── .env                       # Environment variables (not committed)
├── .gitignore
├── package.json
└── README.md
```

## 🏁 Getting Started

### 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/jhonath1010/full-stack-e-commerce-web-app.git
   cd full-stack-e-commerce-web-app
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

### 🔐 Environment Variables

Create a `.env` file in the root directory and add:

```
MONGO_URI=mongodb+srv://<username>:<password>@serverdb.uwnrpwm.mongodb.net/web322db?retryWrites=true&w=majority&tls=true
```

> ⚠️ Replace `<username>` and `<password>` with your actual credentials. Do **not** expose real values in public repositories.

### ▶️ Running the App

```bash
node server.js
```

Visit: `http://localhost:8080`

## 📄 License

This project is licensed under the MIT License.


## 🚀 Deployment

This project was deployed using **Render**. To deploy it yourself, follow these steps:

1. Fork or clone this repository.
2. Push it to your GitHub account.
3. Connect your GitHub repo to [Render](https://render.com/).
4. In the Render dashboard, add the required environment variable `MONGO_URI`.
5. Deploy the web service.

## 🌐 Live Demo

Check out the live version here:  
🔗 [Full-Stack E-Commerce App on Render](https://full-stack-e-commerce-web-app-l1f7.onrender.com/shop)

## 🙏 Acknowledgments

- Inspired by real-world e-commerce app architectures.
- Thanks to the developers of Node.js, Express, MongoDB, PostgreSQL, and all open-source packages used.
