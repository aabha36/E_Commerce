# E_Commerce Mern Stack
Here's a sample **README.md** for your **MERN stack video streaming platform** project. It includes the MongoDB setup, Cloudinary API, PayPal API, and step-by-step instructions for installation:

---

# **Video Streaming Platform**

## **Overview**
This project is a video streaming platform built using the MERN (MongoDB, Express, React, Node.js) stack, offering features like live streaming, Video on Demand (VOD), user authentication, content management, and secure payments via PayPal.

## **Technologies**
- **MongoDB**: NoSQL database for storing user data, videos, and content metadata.
- **Express.js**: Server-side framework for handling API requests.
- **React.js**: Frontend framework for building the user interface.
- **Node.js**: JavaScript runtime for the backend logic.
- **Cloudinary**: Cloud storage and media management for video uploads.
- **PayPal API**: Integrated for handling secure payments.
- **JWT (JSON Web Tokens)**: For user authentication.

## **Prerequisites**
Before starting, ensure you have the following installed:
- **Node.js** (v14 or higher)
- **npm** (v6 or higher)
- **MongoDB Atlas** account (for cloud database)
- **Cloudinary** account (for media uploads)
- **PayPal Developer** account (for payment integration)

## **Environment Variables**
Create a `.env` file in the root of your project to store your API keys and sensitive data.

```bash
# MongoDB connection URI
MONGO_URI=your_mongodb_connection_string

# Cloudinary credentials
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

# PayPal credentials
PAYPAL_CLIENT_ID=your_paypal_client_id
PAYPAL_SECRET=your_paypal_secret

# JWT Secret
JWT_SECRET=your_jwt_secret

# Other settings
PORT=5000
```

### **MongoDB Setup**
1. Sign up at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).
2. Create a new cluster and database.
3. Get your **MongoDB URI** (connection string) from the "Connect" tab in your cluster dashboard.
4. Paste the MongoDB URI into the `.env` file as `MONGO_URI`.

### **Cloudinary Setup**
1. Sign up at [Cloudinary](https://cloudinary.com/).
2. Go to your Cloudinary dashboard to get your **Cloud Name**, **API Key**, and **API Secret**.
3. Add these details to your `.env` file as `CLOUDINARY_CLOUD_NAME`, `CLOUDINARY_API_KEY`, and `CLOUDINARY_API_SECRET`.

### **PayPal Setup**
1. Sign up at [PayPal Developer](https://developer.paypal.com/).
2. Create a new app in the sandbox environment.
3. Get your **Client ID** and **Secret** from the dashboard.
4. Add these details to your `.env` file as `PAYPAL_CLIENT_ID` and `PAYPAL_SECRET`.

## **Installation and Setup**

### **1. Clone the Repository**
```bash
git clone https://github.com/jyoti23456/E_Commerce.git
cd E_Commerce
```

### **2. Install Dependencies**
Install server-side and client-side dependencies:

```bash
# Install backend dependencies
npm install

# Navigate to the frontend directory
cd client

# Install frontend dependencies
npm install
```

### **3. Configure Environment Variables**
Ensure your `.env` file is properly configured with all necessary API keys.

### **4. Run the Development Server**
Start the server and client concurrently using the following:

```bash
# Go back to the root directory
cd ..

# Start both frontend and backend
npm run dev
```

### **5. Building the App for Production**
To build the app for production:

```bash
# Build frontend assets
cd client
npm run build

# Go back to the root directory and run the production server
cd ..
npm run dev
```

## **Features**
- **User Authentication**: Secure user sign-up and login using JWT.
- **Video Streaming**: Supports both live streaming and video on demand (VOD) functionality.
- **Cloudinary Integration**: Handles video uploads and management.
- **Payment Integration**: Secure payments via PayPal API.
- **Content Management**: Allows admins to manage content, including video uploads, descriptions, and schedules.

## **API Endpoints**

| Method | Endpoint           | Description                             |
|--------|--------------------|-----------------------------------------|
| POST   | `/api/auth/register` | Register a new user                    |
| POST   | `/api/auth/login`    | User login                             |
| GET    | `/api/videos`        | Fetch all available videos             |
| POST   | `/api/videos/upload` | Upload a new video                     |
| POST   | `/api/payments`      | Process a PayPal payment               |

## **Contributing**
If you want to contribute to this project, follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push the branch (`git push origin feature-name`).
5. Open a Pull Request.

---
