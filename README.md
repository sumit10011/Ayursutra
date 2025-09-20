# AyurSutra - Panchakarma Patient Management & Therapy Scheduling Software

A comprehensive full-stack web application for Ayurveda wellness centers, Panchakarma clinics, and hospitals. The platform supports separate access for Patients, Doctors/Therapists, and Admins with role-based authentication and comprehensive management features.

## 🌟 Features

### Core Features
- **Authentication & Role-based Access**: JWT-based authentication for Patients, Doctors/Therapists, and Admins
- **Patient Management**: Store patient details, Prakriti (body constitution), medical history, therapy plans
- **Therapy Scheduling System**: Book Panchakarma therapies (Vamana, Virechana, Basti, Nasya, Raktamokshana)
- **Therapist & Resource Allocation**: Smart allocation of available therapists and therapy rooms
- **Inventory Management**: Track Ayurvedic oils, herbs, medicines, consumables
- **Billing & Reports**: Integrated billing for patients with exportable reports
- **Reminders & Notifications**: Email/SMS reminders for patients and notifications for staff
- **Analytics Dashboard**: Insights on patient inflow, therapy demand, revenue trends

### User Roles
- **Patient**: Register → View therapies → Book therapy → Get reminders → View progress
- **Doctor/Therapist**: Approve schedules → See daily sessions → Update patient progress
- **Admin**: Manage patients, doctors, inventory, billing, reports, and dashboard

## 🛠️ Technology Stack

### Frontend
- **React 18** with modern hooks and functional components
- **Tailwind CSS** for beautiful, responsive UI design
- **React Router** for navigation
- **Axios** for API communication
- **React Hot Toast** for notifications
- **Lucide React** for icons
- **Recharts** for analytics and charts

### Backend
- **Node.js** with Express.js framework
- **MongoDB** with Mongoose ODM
- **JWT** for authentication
- **bcryptjs** for password hashing
- **Express Validator** for input validation
- **Nodemailer** for email notifications
- **Twilio** for SMS integration

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or cloud instance)
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd ayursutra
   ```

2. **Install dependencies**
   ```bash
   npm run install-all
   ```

3. **Environment Setup**
   ```bash
   # Copy environment file
   cp server/.env.example server/.env
   
   # Edit server/.env with your configuration
   MONGODB_URI=mongodb://localhost:27017/ayursutra
   JWT_SECRET=your_jwt_secret_key_here
   JWT_EXPIRE=7d
   PORT=5000
   NODE_ENV=development
   ```

4. **Start the application**
   ```bash
   # Start both frontend and backend
   npm run dev
   
   # Or start individually
   npm run server  # Backend only
   npm run client  # Frontend only
   ```

5. **Access the application**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000

## 📱 Login Page Features

The login page includes:
- **Beautiful Design**: Modern, responsive design with Ayurveda-inspired color scheme
- **Role Selection**: Choose between Patient and Doctor/Therapist during registration
- **Form Validation**: Real-time validation with helpful error messages
- **Password Visibility Toggle**: Show/hide password functionality
- **Responsive Layout**: Works perfectly on desktop, tablet, and mobile devices
- **Smooth Animations**: Fade-in and slide-up animations for better UX
- **Accessibility**: Proper ARIA labels and keyboard navigation support

## 🎨 Design Highlights

- **Ayurveda-inspired Color Palette**: Sage green, warm gold, and calming blues
- **Typography**: Inter for body text, Playfair Display for headings
- **Gradient Backgrounds**: Beautiful gradients for visual appeal
- **Card-based Layout**: Clean, modern card design for content organization
- **Icon Integration**: Lucide React icons throughout the interface
- **Responsive Grid System**: Tailwind CSS grid for perfect layouts

## 📁 Project Structure

```
ayursutra/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # Reusable components
│   │   ├── contexts/       # React contexts (Auth)
│   │   ├── pages/          # Page components
│   │   └── layouts/        # Layout components
│   ├── public/             # Static assets
│   └── package.json
├── server/                 # Node.js backend
│   ├── models/             # MongoDB models
│   ├── routes/             # API routes
│   ├── middleware/         # Custom middleware
│   ├── config/             # Configuration files
│   └── package.json
└── package.json            # Root package.json
```

## 🔐 Authentication Flow

1. **Registration**: Users can register as Patient or Doctor/Therapist
2. **Login**: JWT-based authentication with role-based access
3. **Protected Routes**: Role-based route protection
4. **Token Management**: Automatic token refresh and logout

## 🚧 Development Status

### ✅ Completed
- Project structure setup
- Beautiful login page with role-based registration
- JWT authentication system
- Basic dashboard layouts for all user roles
- Responsive design with Tailwind CSS
- Backend API structure with MongoDB models

### 🚧 In Progress
- Patient management system
- Therapy scheduling functionality
- Inventory management
- Billing system
- Notifications system
- Analytics dashboard

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Ayurveda principles and Panchakarma therapy knowledge
- Modern web development best practices
- Open source community for amazing tools and libraries

---

**AyurSutra** - Bridging ancient wisdom with modern technology for holistic wellness management.
