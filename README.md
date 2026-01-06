# 🏥 MedNexus - Hospital Management System (HMS)

MedNexus is a comprehensive **Hospital Management System** designed to streamline healthcare operations. It features role-based access control for **Admins, Doctors, and Patients**, allowing efficient management of appointments, medical records, pharmacy inventory, and hospital analytics.

---

## 🚀 Live Demo

| Component | URL | Status |
| :--- | :--- | :--- |
| **Frontend (Live Site)** | [https://mednexus-hms.vercel.app](https://mednexus-hms.vercel.app) | 🟢 Live |
| **Backend (API)** | [https://mednexus-hms.onrender.com](https://mednexus-hms.onrender.com) | 🟢 Live |

---

## ✨ Key Features

* **🔐 Role-Based Authentication:** Secure login/signup for Admins, Doctors, and Patients using `Passport.js`.
* **👨‍⚕️ Doctor Dashboard:** Manage patient appointments and medical records.
* **📅 Appointment Booking:** Patients can book, view, and track appointments.
* **💊 Pharmacy Management:** Inventory tracking for medicines.
* **📊 Analytics & Charts:** Visual data representation using `Recharts` for hospital insights.
* **🛡️ Protected Routes:** Secure client-side routing using `React Router`.
* **📱 Responsive Design:** Built with `TailwindCSS` for a seamless experience on all devices.

---

## 🛠️ Tech Stack

### **Frontend**
* **Framework:** React.js (Vite)
* **Styling:** TailwindCSS
* **Routing:** React Router DOM
* **HTTP Client:** Axios
* **Charts:** Recharts
* **Icons:** React Icons / FontAwesome

### **Backend**
* **Runtime:** Node.js
* **Framework:** Express.js
* **Database:** MongoDB (via Mongoose)
* **Authentication:** Passport.js (Local Strategy), Express Session
* **Security:** CORS, BCryptJS (Password Hashing)

### **Deployment**
* **Frontend:** Vercel
* **Backend:** Render
* **Database:** MongoDB Atlas

---

## ⚙️ Environment Variables

To run this project locally, you will need to add the following environment variables to your `.env` files.

### **Backend (`backend/.env`)**
Create a `.env` file in the `backend` folder:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
SECRET=your_session_secret_key
VF_URL=http://localhost:5173  # Change to Vercel URL in production

# Admin Configuration (Required for Admin Login)
ADMIN_USERNAME=muffy
ADMIN_PASSWORD=your_secure_password
ADMIN_ID=admin_user_123
ADMIN_ROLE=admin
```

### **Frontend (`frontend/.env`)**
Create a `.env` file in the `frontend` folder:

```env
VITE_API_URL=[https://mednexus-backend.onrender.com](https://mednexus-backend.onrender.com) # Change to Render URL in production
