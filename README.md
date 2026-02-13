Here is a fully professional, high-impact README for your **AutoPark** project. I have optimized the formatting, added professional badges, and structured it to look like a top-tier GitHub repository.

---

# 🚗 AutoPark – Smart Parking Management System

<p align="center">
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP Badge">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL Badge">
  <img src="https://img.shields.io/badge/XAMPP-FB6305?style=for-the-badge&logo=xampp&logoColor=white" alt="XAMPP Badge">
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge" alt="MIT License Badge">
</p>

<p align="center">
<b>A comprehensive web-based solution for automated parking reservations, secure payments, and multi-role management.</b>
<br />
<a href="[https://github.com/WhyNotNarayan/AutoPark](https://www.google.com/search?q=https://github.com/WhyNotNarayan/AutoPark)"><strong>Explore Documentation »</strong></a>
<br />
<br />
<a href="#-system-workflow">View Workflow</a>
·
<a href="[https://github.com/WhyNotNarayan/AutoPark/issues](https://www.google.com/search?q=https://github.com/WhyNotNarayan/AutoPark/issues)">Report Bug</a>
·
<a href="[https://github.com/WhyNotNarayan/AutoPark/issues](https://www.google.com/search?q=https://github.com/WhyNotNarayan/AutoPark/issues)">Request Feature</a>
</p>

---

## 📖 Project Overview

**AutoPark** is an intelligent parking management ecosystem designed to bridge the gap between parking owners and vehicle drivers. Built using a robust **PHP & MySQL** architecture, it eliminates manual errors by providing real-time slot tracking, secure OTP verification, and integrated payment processing.

### Why AutoPark?

In urban environments, finding parking is a major challenge. AutoPark digitizes the entire process—from searching for a slot to extending booking time—ensuring a seamless experience for users and high efficiency for parking owners.

---

## ✨ Key Features

### 👤 User (Customer) Module

* **Secure Onboarding:** Registration with **OTP Verification** via PHPMailer.
* **Smart Booking:** Real-time slot selection and reservation.
* **Integrated Payments:** Mock payment gateway for booking confirmation.
* **Flexibility:** Options to **Extend** or **Cancel** bookings directly from the dashboard.

### 🏢 Owner Module

* **Slot Management:** Real-time status updates (Occupied/Available) for floors and slots.
* **Offline Entry:** Ability to manually add walk-in parking records.
* **Request Tracking:** Manage and approve user booking requests efficiently.

### 🛠️ Admin Panel

* **Global Overview:** Monitor all users, owners, and parking transactions.
* **System Integrity:** Manage expired bookings and handle system-wide requests.
* **Database Control:** Full CRUD capabilities for maintaining system health.

---

## 🛠️ Tech Stack

| Layer | Technology |
| --- | --- |
| **Backend** | PHP (Version 7.4+) |
| **Database** | MySQL |
| **Frontend** | HTML5, CSS3, JavaScript |
| **Authentication** | PHPMailer (SMTP-based OTP) |
| **Environment** | XAMPP / WAMP / Apache |

---

## 📂 Project Structure

```text
Autopark/
├── PHPMailer/           # Secure Email handling library
├── assets/              # CSS, JS, and Image files
├── db/                  # SQL database export files
├── db_config.php        # Database connection settings
├── login.php            # Unified login for all roles
├── user_dashboard.php   # Customer interface
├── owner_dashboard.php  # Parking owner interface
├── admin_dashboard.php  # System administrator interface
├── send_otp.php         # OTP generation logic
└── verify_otp.php       # Verification logic

```

---

## ⚙️ Installation Guide

Follow these steps to get your local development environment running:

1. **Clone the Repository**
```bash
git clone https://github.com/WhyNotNarayan/AutoPark.git

```


2. **Setup Local Server**
* Move the `Autopark` folder to your XAMPP `htdocs` directory.
* Start **Apache** and **MySQL** from the XAMPP Control Panel.


3. **Database Configuration**
* Open `phpMyAdmin` (http://localhost/phpmyadmin).
* Create a new database named `autopark`.
* Import the `.sql` file found in the `/db` folder.


4. **Configure Environment**
* Open `db_config.php` and update your credentials:


```php
$servername = "localhost";
$username = "root";
$password = "";
$database = "autopark";

```


5. **Run the Application**
* Navigate to `http://localhost/Autopark/` in your browser.



---

## 🔄 System Workflow

1. **Authentication:** User signs up → Receives OTP via Email → Account Verified.
2. **Discovery:** User searches for available slots in the dashboard.
3. **Transaction:** User books a slot → Redirected to Payment → Booking Confirmed.
4. **Verification:** Owner verifies the booking upon vehicle arrival.
5. **Completion:** User exits → Slot status automatically reverts to "Available."

---

## 🔮 Future Enhancements

* [ ] **QR Code Integration:** Contactless entry and exit verification.
* [ ] **Live Map API:** Integration with Google Maps for real-time navigation to slots.
* [ ] **SMS Gateway:** Alternative to Email OTP for faster verification.
* [ ] **Advanced Analytics:** Revenue charts for owners and admins.

---

## 👨‍💻 Developed By

**Narayan Ashok Gawade**
<p>
**B.Sc. Computer Science**
</p>

> Passionate about Web Development & Smart Automation Systems.

---

## 📜 License

Distributed under the **MIT License**. See `LICENSE` for more information.

<p align="center">
<b>If this project helped you, please give it a ⭐ on GitHub!</b>
</p>
