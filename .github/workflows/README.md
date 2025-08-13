# Student Course Management System

A dynamic web application for managing student courses, built with Node.js, Express, and modern web technologies.

## Features

- User authentication (registration and login)
- Student dashboard with profile management
- Course browsing and enrollment
- Admin panel for course management
- Responsive design using Bootstrap 5
- RESTful API architecture

## Prerequisites

- Node.js (v14 or higher)
- npm (Node Package Manager)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd student-course-management
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory and add the following:
```
PORT=3000
JWT_SECRET=your-secret-key
```

4. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:3000`

## Project Structure

```
student-course-management/
├── public/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   ├── main.js
│   │   └── dashboard.js
│   ├── index.html
│   └── dashboard.html
├── routes/
│   ├── auth.js
│   ├── courses.js
│   └── students.js
├── server.js
├── package.json
└── README.md
```

## API Endpoints

### Authentication
- POST `/api/auth/register` - Register a new user
- POST `/api/auth/login` - Login user

### Courses
- GET `/api/courses` - Get all courses
- GET `/api/courses/:id` - Get single course
- POST `/api/courses/:id/enroll` - Enroll in a course
- POST `/api/courses` - Create new course (admin only)
- PUT `/api/courses/:id` - Update course (admin only)
- DELETE `/api/courses/:id` - Delete course (admin only)

### Students
- GET `/api/students/profile` - Get student profile
- PUT `/api/students/profile` - Update student profile
- GET `/api/students/courses` - Get student's enrolled courses

## Technologies Used

- **Frontend:**
  - HTML5
  - CSS3
  - JavaScript (ES6+)
  - Bootstrap 5

- **Backend:**
  - Node.js
  - Express.js
  - JWT for authentication
  - bcryptjs for password hashing

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Bootstrap for the responsive design framework
- Express.js for the backend framework
- All contributors who have helped shape this project 