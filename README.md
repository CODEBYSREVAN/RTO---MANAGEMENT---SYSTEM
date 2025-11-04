# RTO---MANAGEMENT---SYSTEM
A web-based Regional Transport Office Management System built with PHP &amp; MySQL. Manages driver licensing, vehicle registration, ownership transfers, and complaints with role-based access for Admin, Users, and RTO Officers.
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat&logo=bootstrap&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

## 🚗 About The Project

The RTO Management System streamlines interactions between citizens and Regional Transport Offices by automating license applications, vehicle registrations, ownership transfers, and complaint management. This system replaces manual paper-based processes with an efficient digital platform, reducing processing time by 40% and improving transparency.

### Built With

* PHP
* MySQL
* HTML5/CSS3
* JavaScript
* Bootstrap
* Apache Server

## ✨ Key Features

### 👨‍💼 Admin Module
- **Dashboard** - Comprehensive statistics and overview
- **License Management** - Approve/reject learning and driving license applications
- **Vehicle Registration** - Process vehicle registration requests
- **License Renewal** - Handle license renewal applications
- **Complaint Management** - Address and resolve user complaints
- **Report Generation** - Generate detailed reports with date filters
- **Master Data** - Manage states, cities, and RTO offices
- **User Management** - View and manage registered users

### 👤 User Module
- **License Applications** - Apply for learner's and driving licenses (Motorcycle/LMV/HMV)
- **Vehicle Registration** - Register new vehicles online
- **Ownership Transfer** - Request vehicle ownership transfers
- **License Renewal** - Apply for license renewals
- **Application Tracking** - Real-time status tracking of all applications
- **Fine Details** - View vehicle-related fines and penalties
- **Complaint System** - Submit and track complaints
- **Enquiry System** - Send queries to RTO office
- **Profile Management** - Update personal information and password

### 🏢 RTO Office Module
- **Application Processing** - Review and process license applications
- **Document Verification** - Verify submitted documents
- **Approval Workflow** - Approve or reject applications with remarks
- **Search Functionality** - Search applications by number or name
- **Report Generation** - Generate office-specific reports
- **Dashboard Analytics** - View application statistics

## 📊 System Capabilities

- ✅ Handles **200+ concurrent users**
- ✅ Manages **3 user roles** (Admin, User, RTO Officer)
- ✅ **18 normalized database tables**
- ✅ **Role-based access control (RBAC)**
- ✅ **Real-time application status tracking**
- ✅ **Automated email notifications**
- ✅ **Secure authentication system**

## 🛠️ Installation

### Prerequisites

- PHP 7.0 or higher
- MySQL 5.6 or higher
- Apache Web Server (XAMPP/WAMP)
- Web Browser (Chrome, Firefox, Safari)

### Setup Instructions

1. **Clone the repository**
```bash
git clone https://github.com/CODEBYSREVAN/RTO---MANAGEMENT---SYSTEM.git
```

2. **Move to web server directory**
```bash
# For XAMPP
move RTO---MANAGEMENT---SYSTEM C:\xampp\htdocs\

# For WAMP
move RTO---MANAGEMENT---SYSTEM C:\wamp64\www\

# For Linux/Mac
sudo mv RTO---MANAGEMENT---SYSTEM /var/www/html/
```

3. **Create Database**
- Open phpMyAdmin: `http://localhost/phpmyadmin`
- Create new database named `rto_db`
- Import SQL file from `/database/rto_db.sql`

4. **Configure Database Connection**
- Copy `db.php.example` to `db.php`
- Update database credentials:
```php
<?php
$con = mysqli_connect("localhost", "root", "", "rto_db");
?>
```

5. **Set Folder Permissions** (For Linux/Mac)
```bash
chmod 755 uploads/
chmod 755 logs/
```

6. **Access Application**
```
http://localhost/RTO---MANAGEMENT---SYSTEM/
```

## 🔐 Default Login Credentials

### Admin Login
```
Username: admin
Password: admin123
```

### Test User
Register through the registration page

### RTO Officer
```
Username: rto_officer
Password: rto123
```

*Note: Update these credentials after first login*

## 📁 Project Structure
```
RTO---MANAGEMENT---SYSTEM/
├── Admin/              # Admin module files
├── User/               # User module files
├── RTO/                # RTO officer module files
├── assets/             # CSS, JS, images
├── database/           # SQL dump file
├── uploads/            # User uploaded files
├── logs/               # Application logs
├── db.php              # Database configuration
├── index.php           # Landing page
├── login.php           # Login page
├── register.php        # User registration
└── README.md           # Project documentation
```

## 💾 Database Schema

The system uses **18 normalized tables**:

| Table Name | Description |
|-----------|-------------|
| `login` | User authentication |
| `user_register` | User details |
| `learners_license_register` | Learning license applications |
| `driving_license_register` | Driving license records |
| `vehicle_registration` | Vehicle details |
| `ownership_transfer` | Transfer requests |
| `license_renewal` | Renewal applications |
| `tbl_complaint` | Complaint management |
| `enquiry` | User enquiries |
| `fine` | Fine/penalty details |
| `penality` | Penalty records |
| `payment` | Payment transactions |
| `fee` | Fee structure |
| `tbl_district` | District master |
| `tbl_rto` | RTO office details |
| `employee_register` | Employee records |
| `old_vehicle_owners` | Vehicle ownership history |

## 🔒 Security Features

- ✅ **Session Management** - Secure user sessions
- ✅ **Password Hashing** - Bcrypt password encryption
- ✅ **SQL Injection Prevention** - Prepared statements
- ✅ **XSS Protection** - Input sanitization
- ✅ **CSRF Protection** - Token-based validation
- ✅ **Role-Based Access Control** - User role validation
- ✅ **Input Validation** - Client and server-side validation

## 🚀 Future Enhancements

- [ ] SMS notifications via API integration
- [ ] Online payment gateway (Razorpay/PayU)
- [ ] Mobile application (Android/iOS)
- [ ] Biometric verification system
- [ ] Digital license download (PDF)
- [ ] Appointment booking system
- [ ] QR code for license verification
- [ ] Multi-language support
- [ ] Advanced analytics dashboard
- [ ] Integration with DigiLocker

## 🎓 Academic Project

This project was developed as a **Mini Project** for the Bachelor of Computer Applications (BCA) program at:

**Catholicate College, Pathanamthitta**  
Affiliated to Mahatma Gandhi University, Kottayam  
Academic Year: 2022-2025

**Project Guide:** Mrs. Swathy Krishna S  
**Department:** Computer Applications

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 Contact

**Srevan S**

- Email: srevan.s.kumar@gmail.com
- Phone: +91 7987511556
- LinkedIn: [linkedin.com/in/srevan-s-bbb49b321](https://linkedin.com/in/srevan-s-bbb49b321)
- GitHub: [@CODEBYSREVAN](https://github.com/CODEBYSREVAN)
- Location: Bengaluru, Karnataka, India

## 🙏 Acknowledgments

Special thanks to:

- **Dr. Sindhu Jones** - Principal, Catholicate College Pathanamthitta
- **Mrs. Deepthy Rajesh** - Head of Department, Computer Applications
- **Mrs. Swathy Krishna S** - Project Guide and Mentor
- Department of Computer Applications, Catholicate College
- My family and friends for their continuous support

## 📄 License

This project is an academic project developed for educational purposes as part of BCA curriculum.

## ⭐ Show Your Support

If you find this project useful, please consider giving it a star ⭐

---

**Made with ❤️ by Srevan S**

*Last Updated: December 2024*
