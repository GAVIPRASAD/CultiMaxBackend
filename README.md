# CultiMax - Backend Application

![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)

**CultiMax** is a dynamic, lightweight, and mobile-compatible web application designed to help farmers buy agricultural products at the right time. This repository contains the server-side logic (Backend) built with the MERN stack.

## 🔗 Live Demo & Resources

- **🌐 Live Website**: [http://cultimax.onrender.com/](http://cultimax.onrender.com/)
- **💻 Frontend Repository**: [GAVIPRASAD/CultiMaxUI](https://github.com/GAVIPRASAD/CultiMaxUI)

## 📋 Table of Contents

- [Features](#-features)
- [Screenshots](#-screenshots)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Server](#running-the-server)
- [API Endpoints](#-api-endpoints)
- [Contributing](#-contributing)

## 🚀 Features

- **Product Management**: Backend logic to handle product listings (Seeds, Fertilizers, Tools).
- **User Authentication**: Secure registration and login handling.
- **Cart Logic**: APIs to manage user shopping carts.
- **Dynamic & Fast**: Optimized endpoints for quick data retrieval.
- **Dockerized**: Ready for containerized deployment.

## 📸 Screenshots

Here are some glimpses of the application in action:

### Home Page
![Home Page](https://user-images.githubusercontent.com/112298797/224025880-1e149f44-7eab-4447-9a4d-a1011e55e0e7.png)

### Products Catalog
![ProductsPart](https://user-images.githubusercontent.com/112298797/224025963-a704e39c-f453-4893-804a-3a2b310a6b71.png)

### Specific Categories (e.g., Seeds)
![Seeds](https://user-images.githubusercontent.com/112298797/224025975-33679161-16cd-42ab-b0ce-5a59db85e2cf.png)

### Shopping Cart
![Cart](https://user-images.githubusercontent.com/112298797/224026015-bffd468d-7320-489f-b795-3efe494f6f1f.png)

### User Dashboard
![Dashboard](https://user-images.githubusercontent.com/112298797/224026038-61f6a745-eede-4768-ade6-9e559312f276.png)

## 🛠 Tech Stack

- **Runtime**: [Node.js](https://nodejs.org/)
- **Framework**: [Express.js](https://expressjs.com/)
- **Database**: [MongoDB](https://www.mongodb.com/)
- **Containerization**: [Docker](https://www.docker.com/)
- **Deployment**: Render (implied by live link)

## 📂 Project Structure

```bash
CultiMaxBackend/
├── build/          # Production build artifacts
├── controller/     # Business logic and request handling
├── db/             # Database connection setup
├── middleware/     # Custom middleware (auth, error handling)
├── models/         # Mongoose Data Models (User, Product, etc.)
├── routes/         # API Route definitions
├── utils/          # Helper functions
├── Dockerfile      # Docker configuration
├── app.js          # Application entry point
└── package.json    # Dependencies and scripts
```

## 🏁 Getting Started

Follow these steps to set up the backend locally.

### Prerequisites

- Node.js installed (v14+ recommended)
- MongoDB installed locally or a MongoDB Atlas connection string
- Docker (Optional, for containerized run)

### Installation

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/GAVIPRASAD/CultiMaxBackend.git](https://github.com/GAVIPRASAD/CultiMaxBackend.git)
    cd CultiMaxBackend
    ```

2.  **Install dependencies**
    ```bash
    npm install
    ```

3.  **Environment Configuration**
    Create a `.env` file in the root directory:
    ```env
    PORT=5000
    MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/CultiMax?retryWrites=true&w=majority
    # Add any other keys (JWT_SECRET, etc.) here
    ```

### Running the Server

**Standard Development Mode:**
```bash
npm start
# or if using nodemon
npm run dev
```

**Using Docker:**
```bash
# Build the image
docker build -t cultimax-backend .

# Run the container
docker run -p 5000:5000 cultimax-backend
```

## 🔌 API Endpoints

The API likely follows these standard REST patterns (inspect `routes/` for details):

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| **GET** | `/api/products` | Get all products |
| **POST** | `/api/auth/register` | Register a new user |
| **POST** | `/api/auth/login` | User login |
| **GET** | `/api/cart` | Fetch user cart |
| **POST** | `/api/cart` | Add item to cart |

## 🤝 Contributing

Contributions are welcome!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source.
