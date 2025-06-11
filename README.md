# Video Call Care

A comprehensive telemedicine platform that enables secure video consultations between healthcare professionals and patients.

## 📌 Project Overview

Video Call Care is a full-stack web application built to facilitate remote healthcare consultations through secure video calling. The platform supports appointment scheduling, user management, and real-time communication using WebRTC technology.

## 🚀 Features

- **Secure Video Consultations**: Real-time video calls between healthcare professionals and patients
- **User Authentication**: Secure login/registration system with password reset functionality
- **Appointment Management**: Schedule, view, and manage appointments
- **User Profiles**: Separate interfaces for patients and healthcare professionals
- **Device Selection**: Choose preferred audio and video devices
- **Responsive Design**: Works across desktop and mobile devices

## 🛠️ Technology Stack

### Frontend
- **React.js**: UI library for building the user interface
- **Redux**: State management
- **Socket.io Client**: Real-time communication
- **WebRTC**: Peer-to-peer video streaming
- **Tailwind CSS**: Utility-first CSS framework for styling
- **Axios**: HTTP client for API requests

### Backend
- **Node.js**: JavaScript runtime environment
- **Express.js**: Web application framework
- **MongoDB**: NoSQL database (with Mongoose ODM)
- **Socket.io**: Real-time bidirectional event-based communication
- **JWT**: JSON Web Tokens for authentication
- **Bcrypt**: Password hashing
- **Nodemailer**: Sending emails
- **Multer**: File upload handling

## 📂 Project Structure

```
.
├── client1/               # Frontend React application
│   ├── certs/             # SSL certificates for secure connections
│   ├── public/            # Static assets
│   └── src/               # Source code
│       ├── components/    # React components
│       ├── handlers/      # Event handlers
│       ├── pages/         # Page components
│       ├── redux-elements/# State management
│       ├── services/      # API services
│       ├── utils/         # Utility functions
│       └── webRTCutilities/# WebRTC specific utilities
│
└── server/                # Backend Node.js server
    ├── public/            # Public server files
    │   └── temp/          # Temporary storage
    └── src/               # Source code
        ├── controllers/   # Request handlers
        ├── db/            # Database connection
        ├── middlewares/   # Express middlewares
        ├── models/        # Mongoose models
        ├── routes/        # API routes
        └── utils/         # Utility functions
```

## 🚦 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- MongoDB (local or Atlas)

### Installation

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd Video-Call-Care
   ```

2. **Set up the server**

   ```bash
   cd server
   npm install
   ```

   Create a `.env` file in the server directory with the following variables:
   ```
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   EMAIL_USER=your_email_for_sending_notifications
   EMAIL_PASS=your_email_password
   PORT=5000
   ```

3. **Set up the client**

   ```bash
   cd client1
   npm install
   ```

   Create a `.env` file in the client1 directory with:
   ```
   REACT_APP_API_URL=http://localhost:5000/api
   REACT_APP_SOCKET_URL=http://localhost:5000
   ```

### Running the Application

1. **Start the server**

   ```bash
   cd server
   npm start
   ```

2. **Start the client**

   ```bash
   cd client1
   npm start
   ```

   The application will be available at `https://localhost:3000`

### Production Deployment

1. **Build the client**

   ```bash
   cd client1
   npm run build
   ```

2. **Deploy the server and client to your preferred hosting provider**

   Recommended platforms:
   - Heroku
   - AWS
   - DigitalOcean
   - Vercel (for client)
   - Netlify (for client)

## 🔒 SSL Certificates

For local development, the application uses self-signed SSL certificates located in the `certs` directory. In a production environment, you should replace these with valid certificates from a trusted certificate authority.

## 👥 User Types

1. **Patients**: Can book appointments, join video consultations, and manage their profiles
2. **Healthcare Professionals**: Can manage appointments, conduct consultations, and access patient information

## 📝 License

[Add your license information here]

## 📞 Contact

[Add contact information here]
