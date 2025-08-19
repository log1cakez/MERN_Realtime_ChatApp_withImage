# MERN Real-time Chat Application with Image Sharing

A modern, real-time chat application built with the MERN stack (MongoDB, Express.js, React, Node.js) featuring real-time messaging, image sharing, user authentication, and a responsive design.

## ✨ Features

- **Real-time Messaging**: Instant message delivery using Socket.IO
- **Image Sharing**: Upload and share images in chat conversations
- **User Authentication**: Secure login/signup with JWT tokens
- **User Profiles**: Customizable user profiles and avatars
- **Responsive Design**: Modern UI built with Tailwind CSS and DaisyUI
- **Dark/Light Theme**: Toggle between themes
- **Real-time Status**: Online/offline user status
- **Message History**: Persistent chat history stored in MongoDB
- **Cloud Storage**: Images stored securely on Cloudinary

## 🚀 Tech Stack

### Backend

- **Node.js** with Express.js framework
- **MongoDB** with Mongoose ODM
- **Socket.IO** for real-time communication
- **JWT** for authentication
- **bcryptjs** for password hashing
- **Cloudinary** for image storage
- **CORS** enabled for cross-origin requests

### Frontend

- **React 18** with modern hooks
- **Vite** for fast development and building
- **Tailwind CSS** for styling
- **DaisyUI** for UI components
- **Socket.IO Client** for real-time features
- **React Router** for navigation
- **Zustand** for state management
- **Axios** for HTTP requests
- **React Hot Toast** for notifications

## 📁 Project Structure

```
MERN_Realtime_ChatApp_withImage/
├── backend/                 # Node.js server
│   ├── src/
│   │   ├── controllers/    # Route controllers
│   │   ├── lib/           # Database, socket, and utility functions
│   │   ├── middleware/    # Authentication middleware
│   │   ├── models/        # MongoDB schemas
│   │   ├── routes/        # API routes
│   │   └── index.js       # Server entry point
│   └── package.json
├── frontend/               # React application
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── pages/         # Page components
│   │   ├── store/         # Zustand state stores
│   │   ├── lib/           # Utility functions and API config
│   │   └── App.jsx        # Main application component
│   └── package.json
└── README.md
```

## 🛠️ Installation & Setup

### Prerequisites

- Node.js (v16 or higher)
- MongoDB database
- Cloudinary account (for image storage)

### Backend Setup

1. Navigate to the backend directory:

   ```bash
   cd backend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the backend directory with the following variables:

   ```env
   PORT=5000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

### Frontend Setup

1. Navigate to the frontend directory:

   ```bash
   cd frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

The frontend will run on `http://localhost:5173` and the backend on `http://localhost:5000`.

## 🔧 Environment Variables

Create a `.env` file in the backend directory with these variables:

| Variable                | Description               | Example                             |
| ----------------------- | ------------------------- | ----------------------------------- |
| `PORT`                  | Server port number        | `5000`                              |
| `MONGODB_URI`           | MongoDB connection string | `mongodb://localhost:27017/chatapp` |
| `JWT_SECRET`            | Secret key for JWT tokens | `your_secret_key_here`              |
| `CLOUDINARY_CLOUD_NAME` | Cloudinary cloud name     | `your_cloud_name`                   |
| `CLOUDINARY_API_KEY`    | Cloudinary API key        | `your_api_key`                      |
| `CLOUDINARY_API_SECRET` | Cloudinary API secret     | `your_api_secret`                   |

## 🚀 Usage

1. **Sign Up/Login**: Create an account or log in with existing credentials
2. **Start Chatting**: Begin conversations with other users
3. **Share Images**: Upload and share images in your conversations
4. **Customize Profile**: Update your profile picture and information
5. **Switch Themes**: Toggle between light and dark themes
6. **Real-time Updates**: Experience instant message delivery and status updates

## 📱 Features in Detail

### Authentication

- Secure user registration and login
- JWT-based authentication
- Protected routes and middleware
- Password hashing with bcrypt

### Real-time Communication

- Socket.IO integration for instant messaging
- Online/offline user status
- Real-time message delivery
- Typing indicators

### Image Sharing

- Cloudinary integration for secure image storage
- Support for various image formats
- Optimized image delivery
- Image preview in chat

### User Management

- User profiles with avatars
- Settings page for customization
- Theme switching (light/dark)
- Responsive navigation

## 🔒 Security Features

- JWT token authentication
- Password hashing with bcrypt
- CORS configuration
- Protected API endpoints
- Secure image upload handling

## 🎨 UI/UX Features

- Modern, responsive design
- Tailwind CSS for styling
- DaisyUI component library
- Dark/light theme support
- Loading skeletons and animations
- Toast notifications
- Mobile-friendly interface

## 📊 API Endpoints

### Authentication

- `POST /api/auth/signup` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `GET /api/auth/me` - Get current user

### Messages

- `GET /api/messages/:userId` - Get chat messages
- `POST /api/messages` - Send a message
- `DELETE /api/messages/:messageId` - Delete a message

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Socket.IO for real-time communication
- Cloudinary for image storage
- Tailwind CSS and DaisyUI for styling
- MongoDB and Mongoose for database management
- React community for the amazing ecosystem

## 📞 Support

If you have any questions or need help with the application, please open an issue in the repository.

---

**Happy Chatting! 🚀**
