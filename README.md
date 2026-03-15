# Hotel Management System

A modern, responsive Hotel Management System web application built with HTML, CSS, JavaScript, Node.js, Express, and MongoDB.

## Features

### 1. Admin Login System
- Secure login page with authentication
- Username and password validation
- Logout functionality
- JWT-based session management

### 2. Dashboard
- Overview cards displaying:
  - Total Rooms
  - Available Rooms
  - Booked Rooms
  - Total Guests
- Real-time statistics

### 3. Room Management
- Add, edit, and delete rooms
- Room types: Single, Double, Deluxe, Suite
- Room status: Available, Booked, Maintenance
- Bulk room operations

### 4. Guest Management
- Register new guests
- Store guest details:
  - Name
  - Phone
  - Email
  - Address
- Guest history and search

### 5. Booking System
- Book rooms for guests
- Check-in/Check-out management
- Date range selection
- Automatic room availability updates
- Booking status tracking

### 6. Payment System
- Record payments
- Calculate booking costs
- Payment status tracking (Paid/Pending)
- Payment history

### 7. Reports
- View all bookings
- Room occupancy statistics
- Guest history
- Exportable reports

### 8. User Interface
- Responsive sidebar navigation
- Dashboard with cards and charts
- Data tables with sorting/filtering
- Search functionality
- Mobile and desktop responsive design

### 9. Extra Features
- Dark/Light mode toggle
- Export booking data to CSV/PDF
- Check-in/Check-out notifications
- Real-time updates

## Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT
- **Security**: bcryptjs for password hashing

## Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- npm or yarn

### Setup

1. Clone the repository
```bash
git clone https://github.com/adomjackson2000-alt/hotel-management-system.git
cd hotel-management-system
```

2. Install dependencies
```bash
npm install
```

3. Configure environment variables
```bash
cp .env.example .env
# Edit .env with your configuration
```

4. Start MongoDB
```bash
# Local MongoDB
mongod

# Or use MongoDB Atlas connection string in .env
```

5. Run the application
```bash
# Development mode
npm run dev

# Production mode
npm start
```

The application will be available at `http://localhost:5000`

## Project Structure

```
hotel-management-system/
├── public/
│   ├── index.html
│   ├── login.html
│   ├── dashboard.html
│   ├── rooms.html
│   ├── guests.html
│   ├── bookings.html
│   ├── payments.html
│   ├── reports.html
│   ├── css/
│   │   ├── style.css
│   │   └── responsive.css
│   └── js/
│       ├── app.js
│       ├── auth.js
│       ├── dashboard.js
│       ├── rooms.js
│       ├── guests.js
│       ├── bookings.js
│       ├── payments.js
│       ├── reports.js
│       └── utils.js
├── models/
│   ├── User.js
│   ├── Room.js
│   ├── Guest.js
│   ├── Booking.js
│   └── Payment.js
├── routes/
│   ├── auth.js
│   ├── rooms.js
│   ├── guests.js
│   ├── bookings.js
│   └── payments.js
├── middleware/
│   └── auth.js
├── controllers/
│   ├── authController.js
│   ├── roomController.js
│   ├── guestController.js
│   ├── bookingController.js
│   └── paymentController.js
├── server.js
├── package.json
└── .env.example
```

## API Endpoints

### Authentication
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `GET /api/auth/me` - Get current user

### Rooms
- `GET /api/rooms` - Get all rooms
- `POST /api/rooms` - Create new room
- `PUT /api/rooms/:id` - Update room
- `DELETE /api/rooms/:id` - Delete room

### Guests
- `GET /api/guests` - Get all guests
- `POST /api/guests` - Register new guest
- `PUT /api/guests/:id` - Update guest
- `DELETE /api/guests/:id` - Delete guest

### Bookings
- `GET /api/bookings` - Get all bookings
- `POST /api/bookings` - Create booking
- `PUT /api/bookings/:id` - Update booking
- `DELETE /api/bookings/:id` - Cancel booking

### Payments
- `GET /api/payments` - Get all payments
- `POST /api/payments` - Record payment
- `PUT /api/payments/:id` - Update payment

## Default Credentials

Username: `admin`
Password: `admin123`

⚠️ **Change these credentials in production!**

## Usage

1. **Login**: Use the default credentials to log in
2. **Dashboard**: View overview statistics
3. **Manage Rooms**: Add, edit, or delete rooms
4. **Manage Guests**: Register and manage guest information
5. **Create Bookings**: Book rooms for guests with check-in/check-out dates
6. **Process Payments**: Record payments for bookings
7. **View Reports**: Generate reports and statistics
8. **Export Data**: Export bookings to CSV or PDF

## Security Features

- Password hashing with bcryptjs
- JWT token-based authentication
- CORS protection
- Input validation and sanitization
- Secure session management

## Future Enhancements

- Email notifications
- SMS notifications
- Advanced analytics
- Multi-language support
- Payment gateway integration
- Room service management
- Housekeeping management

## License

MIT

## Support

For support and questions, please open an issue on GitHub.

---

**Version**: 1.0.0
**Last Updated**: 2026-03-15