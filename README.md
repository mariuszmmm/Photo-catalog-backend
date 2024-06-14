# 📸 Photo Catalog - Backend

## Description
The backend of the "Photo Catalog" application is built using Node.js and Express.js. It supports user login using tokens and hashed passwords, as well as managing photos stored on the Railway server and data in MongoDB.

## Features
- 🔐 **User login** using tokens
- 🔑 **Password hashing**
- 📁 **Storing photos** on the Railway server
- 🗄️ **Storing data** in MongoDB
- 📡 **API for managing the photo catalog**
- 🛡️ **Different user permission levels** (user, administrator)

## Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/mariuszmmm/photo-catalog-backend
   ```
2. **Navigate to the project directory:**
   ```bash
   cd photo-catalog-backend
   ```
3. **Install dependencies:**
   ```bash
   npm install
   ```
4. **Create a `.env` file and add the required environment variables:**
   ```env
   MONGO_URI=your_mongo_uri
   JWT_SECRET=your_jwt_secret
   ```
5. **Start the server:**
   ```bash
   npm start
   ```

## Requirements
- Node.js
- npm
- MongoDB

## API Endpoints
- `POST /api/login` - User login
- `POST /api/user/password` - Change user password (authorization required)
- `POST /api/user/add` - Add a new user (authorization required)
- `GET /api/users` - Get list of users
- `GET /api/items` - Get list of items
- `GET /api/example` - Load example items
- `POST /api/items` - Add a new item (authorization required)
- `PUT /api/items/:id` - Edit an item (authorization required)
- `DELETE /api/items/:id` - Delete an item (authorization required)
- `PUT /api/items/:id/removeImage` - Remove an image from an item (authorization required)
- `GET /api/files` - Get list of files
- `GET /api/files/download` - Download all files as a zip
- `GET /api/files/download/:fileName` - Download a specific file

## Frontend Repository
The frontend of the application is in a separate repository: [https://github.com/mariuszmmm/photo-catalog](https://github.com/mariuszmmm/photo-catalog)
