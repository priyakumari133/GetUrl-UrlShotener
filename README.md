# GET URL - A URL Shortener Application (MERN Stack)

## Overview
GET URL is a full-stack URL shortening application built using the MERN stack. This application allows users to shorten long URLs into manageable links, track analytics, and optimize their web experience.

## Features
- Shorten long URLs into concise, shareable links.
- Store and manage shortened URLs in a MongoDB database.
- Redirect users from short URLs to their original destinations.
- Track usage statistics such as the number of clicks.
- User authentication for personalized URL management.

## Tech Stack
- **Frontend:** React.js, Tailwind CSS
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Mongoose for ORM)
- **Authentication:** JWT (JSON Web Token)

## Installation

### Prerequisites
Ensure you have the following installed on your system:
- Node.js (v16+ recommended)
- MongoDB (local or cloud-based, e.g., MongoDB Atlas)
- Git

### Steps to Run the Project

#### 1. Clone the Repository
```sh
git clone https://github.com/yourusername/url-shortener.git
cd url-shortener
```

#### 2. Install Dependencies
##### Backend
```sh
cd server
npm install
```
##### Frontend
```sh
cd ../client
npm install
```

#### 3. Set Up Environment Variables
Create a `.env` file in the `server` directory and add the following:
```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
BASE_URL=http://localhost:5000
```

#### 4. Run the Application
##### Start the Backend Server
```sh
cd server
npm start
```
##### Start the Frontend Application
```sh
cd ../client
npm start
```

The application will be running on `http://localhost:3000`.

## API Endpoints
### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user and receive JWT token

### URL Shortening
- `POST /api/url/shorten` - Shorten a long URL
- `GET /:shortUrl` - Redirect to the original URL

### Analytics
- `GET /api/url/:id` - Get URL details including click count


## License
This project is licensed under the MIT License.

