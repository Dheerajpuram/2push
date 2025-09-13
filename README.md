# Telecom Subscription Management System

A complete full-stack application for managing telecom subscriptions with user authentication, admin dashboard, and subscription management features.

## 🚀 Features

### Backend (Flask + MySQL)
- **User Authentication** - Login/Signup with password hashing
- **Admin Dashboard** - Complete admin management interface
- **User Dashboard** - User subscription management
- **Database Models** - 7 comprehensive tables for complete data management
- **RESTful API** - Clean API endpoints for all operations
- **Audit Logging** - Complete activity tracking and logging
- **CORS Support** - Cross-origin resource sharing enabled

### Frontend (React + Tailwind CSS)
- **Modern UI** - Clean, responsive design with Tailwind CSS
- **User Authentication** - Login and signup forms
- **Dashboard Navigation** - Intuitive navigation between features
- **Landing Pages** - Dedicated pages for all user features
- **Responsive Design** - Works on desktop and mobile devices

### Database Schema
- **Users** - User accounts with role-based access
- **Plans** - Subscription plans with pricing and quotas
- **Subscriptions** - User subscription records
- **Usage** - Data usage tracking
- **Audit Logs** - Activity logging and tracking
- **Discounts** - Promotional offers and discount codes
- **Alerts** - User notifications and alerts

## 🛠️ Tech Stack

### Backend
- **Flask** - Python web framework
- **SQLAlchemy** - ORM for database operations
- **MySQL** - Database management system
- **PyMySQL** - MySQL database connector
- **Werkzeug** - Password hashing and security

### Frontend
- **React** - JavaScript library for building user interfaces
- **React Router** - Client-side routing
- **Tailwind CSS** - Utility-first CSS framework
- **Axios** - HTTP client for API calls

## 📦 Installation

### Prerequisites
- Python 3.7+
- Node.js 14+
- MySQL 5.7+

### Backend Setup
```bash
cd backend
pip install -r requirements.txt
python app.py
```

### Frontend Setup
```bash
cd frontend
npm install
npm start
```

## 🗄️ Database Configuration

Update the database connection in `backend/config.py`:
```python
SQLALCHEMY_DATABASE_URI = 'mysql+pymysql://username:password@localhost/database_name'
```

## 🚀 Running the Application

1. **Start Backend** (Port 5001):
   ```bash
   cd backend
   python app.py
   ```

2. **Start Frontend** (Port 3000):
   ```bash
   cd frontend
   npm start
   ```

3. **Access the Application**:
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5001

## 📁 Project Structure

```
├── backend/
│   ├── models/          # Database models
│   ├── routes/          # API routes
│   ├── services/        # Business logic
│   ├── utils/           # Utility functions
│   ├── app.py           # Flask application
│   └── requirements.txt # Python dependencies
├── frontend/
│   ├── src/
│   │   ├── pages/       # React components
│   │   ├── utils/       # Utility functions
│   │   └── App.js       # Main React component
│   └── package.json     # Node.js dependencies
└── README.md
```

## 🔐 Default Credentials

### Admin
- Email: `admin@example.com`
- Password: `admin123`

### Demo User
- Email: `user@example.com`
- Password: `user123`

## 📊 API Endpoints

### Authentication
- `POST /user/login` - User login
- `POST /user/signup` - User registration
- `POST /admin/login` - Admin login

### User Routes
- `GET /user/dashboard` - User dashboard
- `GET /user/plans-available` - Available plans
- `GET /user/plan-recommendations` - Plan recommendations
- `GET /user/my-plan` - Current plan
- `GET /user/alerts` - User alerts
- `GET /user/discounts` - Available discounts

### Admin Routes
- `GET /admin/dashboard` - Admin dashboard
- `GET /admin/plans` - Manage plans
- `GET /admin/discounts` - Manage discounts
- `GET /admin/users` - Manage users
- `GET /admin/analytics` - Analytics

## 🎯 Features Overview

### User Features
- **Plans Available** - Browse all subscription plans
- **Plan Recommendations** - Get personalized suggestions
- **My Plan** - View current active subscription
- **Alerts** - Important notifications
- **Discounts** - Available offers and promotions

### Admin Features
- **Dashboard** - Overview of system metrics
- **Plan Management** - Create and manage subscription plans
- **Discount Management** - Manage promotional offers
- **User Management** - View and manage users
- **Analytics** - System usage analytics

## 🔧 Development

### Database Migrations
The application uses SQLAlchemy's `create_all()` method to create tables. For production, consider using Flask-Migrate for proper database migrations.

### Environment Variables
Create a `.env` file in the backend directory:
```
DATABASE_URL=mysql+pymysql://username:password@localhost/database_name
SECRET_KEY=your-secret-key-here
```

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📞 Support

For support and questions, please open an issue in the repository.

---

**Note**: This is a demo application for educational purposes. For production use, ensure proper security measures, environment configuration, and database optimization.