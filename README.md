# LinkMe - Social Media App

A modern social media application built with the MERN stack (MongoDB, Express.js, React.js, Node.js) that connects people and enables seamless social interactions.

## 🚀 Features

- **User Authentication**: Secure signup/login with JWT tokens
- **Profile Management**: Create and customize user profiles
- **Post Creation**: Share thoughts, images, and updates
- **Social Interactions**: Like, comment, and share posts
- **Real-time Updates**: Live notifications and feed updates
- **Follow System**: Follow/unfollow other users
- **News Feed**: Personalized content feed
- **Responsive Design**: Mobile-friendly interface

## 🛠️ Tech Stack

**Frontend:**
- React.js
- Redux (State Management)
- Material-UI / Styled Components
- Axios (HTTP Client)

**Backend:**
- Node.js
- Express.js
- JWT Authentication
- Bcrypt (Password Hashing)

**Database:**
- MongoDB
- Mongoose ODM

**Additional Tools:**
- Cloudinary (Image Upload)
- Socket.io (Real-time Features)

## 📋 Prerequisites

Before running this application, make sure you have the following installed:

- Node.js (v14 or higher)
- npm or yarn
- MongoDB (local or MongoDB Atlas)
- Git

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/Sheikhspearee/LinkMe---Social-Media-App-

cd LinkMe---Social-Media-App-
```

### 2. Install Backend Dependencies
```bash
cd backend
npm install
```

### 3. Install Frontend Dependencies
```bash
cd ../frontend
npm install
```

### 4. Environment Variables

Create a `.env` file in the backend directory:

```env
# Database
MONGODB_URI=mongodb://localhost:27017/linkme
# or MongoDB Atlas URI: mongodb+srv://username:password@cluster.mongodb.net/linkme

# JWT Secret
JWT_SECRET=your-super-secret-jwt-key

# Server Port
PORT=5000

# Client URL (for CORS)
CLIENT_URL=http://localhost:3000
```

Create a `.env` file in the frontend directory:

```env
REACT_APP_API_URL=http://localhost:5000/api
REACT_APP_SOCKET_URL=http://localhost:5000
```

## 🚀 Running the Application

### Development Mode

1. **Start the Backend Server:**
```bash
cd backend
npm run dev
```

2. **Start the Frontend Development Server:**
```bash
cd frontend
npm start
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

### Production Mode

1. **Build the Frontend:**
```bash
cd frontend
npm run build
```

2. **Start the Production Server:**
```bash
cd backend
npm start
```

## 📁 Project Structure

```
LinkMe---Social-Media-App-/
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   ├── utils/
│   ├── server.js
│   └── package.json
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── redux/
│   │   ├── utils/
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
│
├── README.md
└── .gitignore
```

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `GET /api/auth/me` - Get current user

### Users
- `GET /api/users/profile/:id` - Get user profile
- `PUT /api/users/profile` - Update user profile
- `POST /api/users/follow/:id` - Follow/unfollow user

### Posts
- `GET /api/posts` - Get all posts
- `POST /api/posts` - Create new post
- `PUT /api/posts/:id` - Update post
- `DELETE /api/posts/:id` - Delete post
- `POST /api/posts/:id/like` - Like/unlike post
- `POST /api/posts/:id/comment` - Add comment

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Development Guidelines

- Follow ES6+ standards
- Use meaningful commit messages
- Write clean, readable code
- Add comments for complex logic
- Test your changes before submitting

## 🐛 Known Issues

- [ ] Real-time notifications may delay on slower connections
- [ ] Image upload size limit needs optimization
- [ ] Mobile responsiveness needs improvement on older devices

## 🔮 Future Enhancements

- [ ] Private messaging system
- [ ] Story feature
- [ ] Advanced search functionality
- [ ] Dark mode toggle
- [ ] Push notifications
- [ ] Video upload support
- [ ] Group/community features

## 👨‍💻 Author

**Your Name**
- GitHub: [@Sheikhspearee](https://github.com/Sheikhspearee/LinkMe---Social-Media-App-)
- LinkedIn: [riyaaz-mahamed](https://linkedin.com/in/riyaaz-mahamed)

## 🙏 Acknowledgments

- React community for excellent documentation
- MongoDB team for the robust database solution
- All contributors who helped improve this project

⭐ **Star this repository if you found it helpful!**
