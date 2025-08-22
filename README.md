# Airbnb Clone

A full-stack web application that replicates core Airbnb functionality, built with Node.js, Express, MongoDB, and EJS templating engine.

## 🚀 Features

- **User Authentication**: Sign up, login, and session management
- **Property Management**: Hosts can add, edit, and manage their properties
- **Property Listings**: Browse available properties with search and filtering
- **Booking System**: Reserve properties with booking management
- **Favorites**: Save and manage favorite properties
- **Image Upload**: Support for property photos with file validation
- **Responsive Design**: Modern UI built with Tailwind CSS

## 🛠️ Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MongoDB with Mongoose ODM
- **Template Engine**: EJS
- **Styling**: Tailwind CSS
- **File Upload**: Multer
- **Authentication**: bcryptjs, express-session
- **Validation**: express-validator

## 📋 Prerequisites

- Node.js (v14 or higher)
- MongoDB database
- npm or yarn package manager

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd airbnb-clone
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   - Update the MongoDB connection string in `app.js`
   - Replace the placeholder connection string with your MongoDB URI

4. **Start the application**
   ```bash
   npm start
   ```

   This will start both the Node.js server and Tailwind CSS watcher.

## 📁 Project Structure

```
airbnb-clone/
├── app.js                 # Main application entry point
├── controllers/           # Business logic controllers
│   ├── authController.js  # Authentication logic
│   ├── hostController.js  # Host property management
│   ├── storeController.js # Property listing and booking
│   └── errors.js         # Error handling
├── models/                # Database models
│   ├── home.js           # Property model
│   └── user.js           # User model
├── routes/                # API routes
│   ├── authRouter.js     # Authentication routes
│   ├── hostRouter.js     # Host management routes
│   └── storeRouter.js    # Property and booking routes
├── views/                 # EJS templates
│   ├── auth/             # Authentication views
│   ├── host/             # Host management views
│   ├── store/            # Property listing views
│   └── partials/         # Reusable template components
├── public/                # Static assets
│   ├── images/           # Property images
│   └── output.css        # Compiled Tailwind CSS
├── uploads/               # User-uploaded files
└── utils/                 # Utility functions
```

## 🔧 Available Scripts

- `npm start` - Start the development server with Tailwind CSS watcher
- `npm run tailwind` - Watch and compile Tailwind CSS
- `npm test` - Run tests (currently not configured)

## 🌐 Usage

1. **Access the application**: Navigate to `http://localhost:3003`
2. **Sign up/Login**: Create an account or sign in to access features
3. **Browse Properties**: View available properties as a guest
4. **Host Properties**: Switch to host mode to add and manage properties
5. **Book Properties**: Reserve properties and manage bookings
6. **Manage Favorites**: Save and organize favorite properties

## 🔐 Authentication

The application uses session-based authentication with MongoDB session storage. Users must be logged in to access host features and make bookings.

## 📸 File Upload

- Supports PNG, JPG, and JPEG image formats
- Images are stored in the `uploads/` directory
- File names are randomized for security

## 🎨 Styling

The application uses Tailwind CSS for styling with a custom configuration. The CSS is compiled from `views/input.css` to `public/output.css`.

## 🚧 Development

- **Port**: 3003 (configurable in `app.js`)
- **Database**: MongoDB with connection string in `app.js`
- **Session Secret**: Configured in the session middleware

