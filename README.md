# 🪪 DVLD - Driving License Management System

A comprehensive desktop application for managing the complete lifecycle of driving license operations, built with **C#**, **Windows Forms**, and **SQL Server**.

## 📋 Overview

DVLD is a robust system designed to streamline the process of issuing, renewing, and managing driving licenses. It provides a secure, scalable platform for government officials to efficiently handle license applications, tests, and renewals.

---

## ✨ Key Features

### 👤 **User Management**
- Role-based access control (Admin, Officer, Clerk)
- Secure authentication and authorization
- User activity logging and audit trails

### 📝 **Application Management**
- License application submission and tracking
- Multi-step verification process
- Document management system
- Fee calculation and payment tracking

### 🧪 **Testing System**
- Vision tests
- Written driving tests
- Practical driving tests
- Test scheduling and result management

### 🔄 **License Operations**
- First-time license issuance
- License renewals
- License replacement/reissuance
- Suspension and revocation management

### 📊 **Reporting & Analytics**
- Comprehensive reporting dashboard
- Application statistics
- Test performance metrics
- Payment tracking reports

### 🔐 **Security & Compliance**
- Data encryption
- Role-based access control
- Audit logging
- Secure database operations with Stored Procedures

---

## 🛠 Tech Stack

- **Language:** C# (.NET Framework)
- **Frontend:** Windows Forms
- **Database:** SQL Server
- **Architecture:** 3-Layer Architecture (Presentation, Business Logic, Data Access)
- **Pattern:** Repository Pattern, OOP Principles

---

## 🏗 Architecture

The application follows a **3-Layer Architecture** for clean separation of concerns:

```
┌─────────────────────────────────┐
│   Presentation Layer (UI)       │
│   - Windows Forms               │
│   - User Interfaces             │
└─────────────────────────────────┘
           ↓
┌─────────────────────────────────┐
│   Business Logic Layer          │
│   - Core Operations             │
│   - Validation & Rules          │
│   - Business Rules Engine       │
└─────────────────────────────────┘
           ↓
┌─────────────────────────────────┐
│   Data Access Layer             │
│   - Database Operations         │
│   - Stored Procedures           │
│   - Data Models                 │
└─────────────────────────────────┘
           ↓
┌─────────────────────────────────┐
│   SQL Server Database           │
│   - Stored Procedures           │
│   - Triggers & Functions        │
└─────────────────────────────────┘
```

---

## 📦 Installation

### Prerequisites
- Windows OS
- .NET Framework 4.7+
- SQL Server 2016 or higher
- Visual Studio 2019+

### Setup Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Aymn-Ahmed/DVLD-Project-.git
   cd DVLD-Project-
   ```

2. **Database Setup**
   - Open SQL Server Management Studio
   - Execute the database script: `Database/DVLD_Database.sql`
   - Configure connection string in `App.config`

3. **Build & Run**
   ```bash
   Open DVLD.sln in Visual Studio
   Build the solution
   Run the application
   ```

---

## 🚀 Usage

### Getting Started

1. **Login**
   - Default credentials: `admin / admin123`
   - Navigate to User Management to create additional users

2. **Application Workflow**
   ```
   New Application → Verify Eligibility → 
   Schedule Tests → Conduct Tests → 
   Issue License → Track & Manage
   ```

3. **Admin Functions**
   - User management
   - System configuration
   - Report generation
   - Audit logs

---

## 💾 Database Schema Highlights

### Key Tables
- `Users` - User accounts and roles
- `Applications` - License applications
- `People` - Applicant information
- `Tests` - Test records
- `Licenses` - Issued licenses
- `TestTypes` - Available test types
- `LicenseClasses` - License classifications

### Stored Procedures
- `sp_AddNewApplication` - Create new application
- `sp_GetApplicationDetails` - Retrieve application info
- `sp_IssueLicense` - Issue new license
- `sp_RenewLicense` - Renew existing license
- `sp_GetUserPermissions` - Retrieve user access

---

## 🔐 Security Features

- **Authentication:** User login with role-based access
- **Authorization:** Permission-based feature access
- **Data Validation:** Input validation at all layers
- **SQL Injection Prevention:** Parameterized queries and Stored Procedures
- **Audit Logging:** Track all critical operations
- **Encryption:** Sensitive data encryption

---

## 📈 Performance Optimizations

- Indexed database queries
- Efficient Stored Procedures
- Lazy loading for large datasets
- Connection pooling
- Query optimization

---

## 📝 Project Structure

```
DVLD-Project/
├── Presentation/
│   ├── Forms/
│   ├── Controls/
│   └── Resources/
├── BusinessLogic/
│   ├── Services/
│   ├── Validators/
│   └── Models/
├── DataAccess/
│   ├── Repositories/
│   ├── Entities/
│   └── Context/
├── Database/
│   ├── Scripts/
│   └── StoredProcedures/
└── README.md
```

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 👨‍💻 Author

**Ayman Ahmed Al-Rajwi**
- 📧 Email: ymn85610@gmail.com
- 💼 LinkedIn: [linkedin.com/in/aymen-alrjwy](https://linkedin.com/in/aymen-alrjwy)
- 🌐 Portfolio: [aymanfullstack.netlify.app](https://aymanfullstack.netlify.app)

---

## 📞 Contact & Support

For questions or support, please reach out:
- 📧 ymn85610@gmail.com
- 📱 +966 50 751 1216

---

<div align="center">

### ⭐ If you find this project useful, please consider giving it a star! ⭐

</div>
