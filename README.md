# 🩺 DocSpot - Doctor Appointment Booking System

# Website Link :
https://docspot-7jfw.onrender.com/


DocSpot is a full-stack web application that enables customers to book appointments with doctors, manage their bookings, and receive reminders. Doctors can manage their schedules, while admins can approve or reject doctor registrations.

---

## ✨ Features

### 👨‍⚕️ For Customers:
- Register and log in securely
- Search for doctors by name or specialization
- Book, reschedule, or cancel appointments
- View past appointments and submit doctor ratings
- OTP-based password recovery

### 🩺 For Doctors:
- View and manage upcoming appointments
- Accept, reject, or mark appointments as completed
- View patient details and history (future scope)

### 🛡️ For Admins:
- Review pending doctor registrations
- Approve or reject doctors with one click

---

## 🧱 Tech Stack

| Layer        | Technology           |
|-------------|----------------------|
| Frontend    | HTML, CSS, JavaScript |
| Backend     | Node.js, Express.js   |
| Database    | MongoDB, Mongoose     |
| Email OTP   | Nodemailer (Gmail SMTP) |
| Deployment  | (Add once hosted)     |

---

## 📁 Folder Structure

```
/public
  /css        → Individual CSS files for each page
  /js         → JavaScript files for page-specific logic
/backend
  /routes     → Express route handlers (auth, user, appointments)
  /models     → Mongoose schemas (User, Appointment)
  /utils      → Email utility for OTP handling
index.html
login.html
register.html
customer-dashboard.html
doctor-dashboard.html
admin-dashboard.html
book-appointment.html
booking-history.html
```

---

## 🔐 Authentication & Role Management

- Users can register as **customers** or **doctors**
- Admin account is created manually (secured & hidden from registration)
- Role-based redirection on login
- OTP-based password recovery with 10-minute expiry

---

## 📅 Appointment Lifecycle

Each appointment has a **status**:
- `pending`
- `accepted`
- `rejected`
- `cancelled`
- `completed`

Customers and doctors see appropriate views and actions based on these statuses.

---

## 📚 Booking History

Customers can:
- View **past appointments**
- See **status tags**
- Submit **1–5 star ratings** for doctors

---

## 🎨 UI/UX Design

- Minimal and clean layout
- Fully responsive for mobile and desktop
- Consistent color palette (healthcare-friendly teal/blue theme)
- Each page styled with its own separate CSS

---

## 🚀 Future Improvements

- Appointment slot management
- Notification system (SMS/Email)
- Admin analytics dashboard
- PDF summary for appointments
- Chat or review system

---

## 🛠️ Setup Instructions

1. Clone the repo
   ```bash
   git clone https://github.com/yourusername/docspot.git
   cd docspot
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Set up `.env`
   ```env
   MONGO_URI=your_mongodb_connection_string
   EMAIL_USER=your_email@example.com
   EMAIL_PASS=your_app_password
   ```

4. Start the server
   ```bash
   npm start
   ```

5. Open `index.html` in your browser to use the frontend.

---

## 🙌 Acknowledgments

- **MongoDB**, **Express**, **Node.js**, and for technology inspiration

---

## 📧 Contact

Have questions or want to collaborate?  
📬 Email:  anushrao9866@gmail.com  
