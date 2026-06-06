# 🎬 BookMyMovie — Movie Ticket Booking System

A full-stack web application for booking movie tickets online, built with Python Flask and MySQL.

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat&logo=python)
![Flask](https://img.shields.io/badge/Flask-2.x-black?style=flat&logo=flask)
![MySQL](https://img.shields.io/badge/MySQL-8.0-orange?style=flat&logo=mysql)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-2.x-38bdf8?style=flat&logo=tailwindcss)

## ✨ Features

- 🔐 User Registration & Login with secure password hashing
- 🎥 Browse movies with Search, Language & Genre filters
- 🪑 Interactive seat selection with real-time availability
- 💳 UPI Payment integration with QR code
- 🎟️ Auto-generated QR ticket after booking confirmation
- 📋 My Bookings — view all past bookings with QR codes
- ⚙️ Admin Dashboard — manage movies, view bookings & revenue

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python, Flask |
| Database | MySQL 8.0 |
| Frontend | HTML5, TailwindCSS, JavaScript |
| Auth | Session-based + SHA256 hashing |
| QR Code | qrcode + Pillow |

## 🚀 Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/MovieTicketBookingSystem.git
cd MovieTicketBookingSystem
```

### 2. Create virtual environment
```bash
python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate  # Mac/Linux
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure environment
Create a `.env` file:
```
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=movie_booking
SECRET_KEY=your_secret_key
ADMIN_PASSWORD=admin123
```

### 5. Setup database
```bash
mysql -u root -p
source path/to/db_setup.sql
```

### 6. Run the app
```bash
python app.py
```
Visit **http://127.0.0.1:5000**

## 📁 Project Structure
```
MovieTicketBookingSystem/
├── app.py              # Flask routes & logic
├── config.py           # Database connection
├── db_setup.sql        # Schema + seed data
├── requirements.txt    # Dependencies
├── .env                # Environment variables (not pushed)
├── static/
│   ├── css/
│   └── images/         # Movie posters + QR codes
└── templates/
    ├── base.html
    ├── index.html
    ├── login.html
    ├── register.html
    ├── movie_detail.html
    ├── book_ticket.html
    ├── payment.html
    ├── success.html
    ├── my_bookings.html
    └── admin_dashboard.html
```

## 👤 Author
Made with ❤️ by [Your Name]
