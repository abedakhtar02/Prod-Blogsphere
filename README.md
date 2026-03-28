# Prod-Blogsphere

A full-stack blogging platform built with Node.js, Express, and MongoDB. Prod-Blogsphere enables users to create, read, update, and delete blog posts with a clean, modern interface.

## 📋 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Scripts](#scripts)
- [API Routes](#api-routes)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

- User authentication with JWT
- Create, read, update, and delete blog posts
- Image upload functionality
- EJS templating for server-side rendering
- Responsive design
- Cookie-based session management
- MongoDB database integration

## 🛠️ Tech Stack

**Backend:**
- Node.js
- Express.js (v5.1.0)
- MongoDB with Mongoose ODM (v8.14.1)
- JWT for authentication (v9.0.2)

**Frontend:**
- EJS (v3.1.10) - Embedded JavaScript templating
- HTML/CSS/JavaScript

**Utilities:**
- Multer (v1.4.5-lts.2) - File upload handling
- Cookie-Parser (v1.4.7) - Cookie management
- Dotenv (v16.5.0) - Environment variables

**Development:**
- Nodemon (v3.1.10) - Auto-reload on file changes

## 📁 Project Structure

```
Prod-Blogsphere/
├── app.js              # Main application entry point
├── connect.js          # Database connection configuration
├── package.json        # Project dependencies
├── middlewares/        # Custom middleware functions
├── models/             # Mongoose schemas and models
├── routes/             # API route definitions
├── services/           # Business logic and services
├── views/              # EJS template files
└── public/             # Static assets (CSS, JS, images)
```

## 📦 Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- MongoDB (local or MongoDB Atlas)

## 🚀 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/abedakhtar02/Prod-Blogsphere.git
   cd Prod-Blogsphere
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Create a `.env` file in the root directory:**
   ```bash
   touch .env
   ```

## ⚙️ Configuration

Create a `.env` file in the root directory with the following variables:

```env
# Database
MONGODB_URI=mongodb://localhost:27017/blogsphere
# or for MongoDB Atlas:
MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/blogsphere

# JWT Secret
JWT_SECRET=your_secret_key_here

# Port
PORT=3000

# Node Environment
NODE_ENV=development
```

## 💻 Usage

### Start the development server:
```bash
npm run dev
```
The application will be available at `http://localhost:3000`

### Start the production server:
```bash
npm start
```

## 📜 Scripts

| Script | Description |
|--------|-------------|
| `npm start` | Start the application in production mode |
| `npm run dev` | Start the application with auto-reload (development mode) |

## 🔌 API Routes

Routes are organized in the `routes/` directory. Available endpoints include:

- **Blog Posts:** Create, read, update, delete blog posts
- **Authentication:** User registration and login
- **User Management:** User profile management

For detailed API documentation, refer to the route files in the `routes/` directory.

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License. See the `package.json` file for more details.

---

**Created by:** [abedakhtar02](https://github.com/abedakhtar02)

**Last Updated:** March 28, 2026
```
