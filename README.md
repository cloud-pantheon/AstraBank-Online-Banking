# 🏦 Banking System Management

A full-stack **Banking System Management Web Application** built with **PHP**, **MySQL**, **HTML**, **CSS**, and **JavaScript**. This project provides secure banking features for users and an admin panel for managing accounts, cards, billers, and transactions.

---

## 🚀 Features

### 👤 User Authentication

* User login system
* OTP verification for secure transactions
* Session-based access control

### 🏦 Account Management

* View account details
* Check account balance
* Manage personal banking information
* Submit phone/email update requests

### 💳 Card Management

* View linked cards
* Manage card information
* Admin can add, update, and manage cards

### 🔁 Bank Transfer

* Transfer money to another bank account
* OTP confirmation before transfer
* Transaction overview before final submission
* Unique reference ID generation

### 📱 MFS Transfer

* Send money to mobile financial services such as:

  * bKash
  * Nagad
  * Rocket
* Receiver wallet name display
* OTP-based confirmation

### 📲 Mobile Recharge

* Recharge mobile numbers
* Operator selection
* OTP verification
* Recharge transaction history

### 🧾 Bill Payment

* Search billers
* Pay utility bills
* OTP confirmation
* Bill payment receipt generation

### 📄 Statement & Receipt

* View transaction history
* Generate PDF bank statements
* Download transaction receipts using FPDF

### 🛠️ Admin Panel

* Manage user accounts
* Manage bank accounts
* Manage cards
* Manage billers
* Review user information update requests
* Monitor transactions

---

## 🛠️ Technologies Used

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** PHP
* **Database:** MySQL
* **Server:** XAMPP / Apache
* **PDF Generation:** FPDF
* **Authentication:** PHP Sessions + OTP Verification

---

## 📁 Project Structure

```text
Banking-System-Web-App/
│
├── admin/
│   ├── admin.php
│   ├── admin_login.php
│   ├── admin_otp.php
│   ├── admin_overview.php
│   ├── admin-add_account.php
│   ├── admin-add_card.php
│   ├── admin-add_biller.php
│   ├── admin-update_account.php
│   ├── admin-update_biller.php
│   ├── admin-update_card_status.php
│   └── admin-get_account_by_cid.php
│
├── auth/
│   ├── login.php
│   ├── signup.php
│   ├── otp.php
│   ├── logout.php
│   └── pass_reset.html
│
├── config/
│   ├── connect.php
│   └── infobip_sms.php
│
├── user/
│   ├── dashboard.php
│   ├── my-cards.php
│   ├── statement.php
│   ├── transaction-history.php
│   ├── certificate.php
│   ├── help-support.php
│   ├── info-update.php
│   ├── info-update-email.php
│   ├── info-update-mobile.php
│   ├── info-update-process.php
│   └── info-update-router.php
│
├── transfers/
│   ├── bank/
│   │   ├── bank-transfer.php
│   │   ├── bank-transfer-process.php
│   │   ├── bank-transfer-overview.php
│   │   ├── bank-transfer-otp.php
│   │   ├── bank-transfer-success.php
│   │   └── bank-transfer-receipt.php
│   │
│   ├── mfs/
│   │   ├── mfs-transfer.php
│   │   ├── mfs-transfer.html
│   │   ├── mfs-transfer-process.php
│   │   ├── mfs-transfer-overview.php
│   │   ├── mfs-transfer-success.php
│   │   ├── mfs-transfer-receipt.php
│   │   ├── get_bkash_name.php
│   │   ├── get_nagad_name.php
│   │   └── get_rocket_name.php
│   │
│   ├── recharge/
│   │   ├── recharge.php
│   │   ├── recharge-overview.php
│   │   ├── recharge-otp.php
│   │   ├── recharge-success.php
│   │   └── recharge-receipt.php
│   │
│   ├── bill-payments/
│   │   ├── bill-payments.php
│   │   ├── bill-billers.php
│   │   ├── bill-amount.php
│   │   ├── bill-category-internet.php
│   │   ├── bill-payment-overview.php
│   │   ├── bill-otp.php
│   │   └── bill-success.php
│   │
│   └── add-money/
│       ├── add-money.php
│       ├── add-money-from.php
│       ├── add-money-to.php
│       ├── add-money-amount.php
│       ├── add-money-overview.php
│       ├── add-money-otp.php
│       ├── add-money-success.php
│       ├── add-money-history.php
│       └── add-money-saved.php
│
├── cards/
│   ├── add-card.php
│   ├── add-card-otp.php
│   └── add-card-success.php
│
├── pdf/
│   ├── statement-pdf.php
│   ├── bill-receipt-pdf.php
│   └── certificate-pdf.php
│
├── products/
│   ├── accounts-savings.html
│   ├── accounts-current.html
│   ├── accounts-fixed.html
│   ├── accounts-dps.html
│   ├── accounts-loan.html
│   ├── accounts-cards.html
│   ├── accounts-nrb.html
│   ├── accounts-others.html
│   ├── accounts-bancassurance.html
│   └── account-*.html
│
├── assets/
│   ├── css/
│   │   ├── style.css
│   │   ├── styles.css
│   │   ├── login.css
│   │   ├── dashboard.css
│   │   ├── products.css
│   │   └── transfer.css
│   │
│   ├── js/
│   │   ├── script.js
│   │   └── scripts.js
│   │
│   ├── images/
│   │   ├── kingfisher-2.png
│   │   ├── Abstract-humming-bird-colorful-logo-on-transparent-background-PNG.png
│   │   └── 594073278_1445243417167154_9032284854136610687_n.jpg
│   │
│   └── pdf/
│       └── Account Certificate.pdf
│
├── vendor/
│   └── fpdf186/
│
├── uploads/
│   └── nid/
│
├── docs/
│   ├── screenshots/
│   ├── ERD.png
│   └── structure.txt
│
├── index.php
├── index.html
├── homepage.html
├── open-account.php
├── astra-locator.php
├── products.html
├── README.md
└── database.sql
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/banking-system.git
```

### 2. Move Project to XAMPP

Move the project folder into:

```text
C:\xampp\htdocs\
```

### 3. Start XAMPP

Start:

* Apache
* MySQL

### 4. Create Database

Open phpMyAdmin:

```text
http://localhost/phpmyadmin
```

Create a database, for example:

```sql
banking_system
```

### 5. Import SQL File

Import the provided `.sql` database file into phpMyAdmin.

### 6. Configure Database Connection

Update your database connection file:

```php
$host = "localhost";
$user = "root";
$password = "";
$database = "banking_system";
```

### 7. Run the Project

Open in browser:

```text
http://localhost/Banking-System/
```

---

## 📊 Main Database Tables

* `user`
* `accounts`
* `cards`
* `billers`
* `transfers`
* `mfs_transfers`
* `recharges`
* `bill_payments`
* `update_requests`

---

## 🔐 Security Features

* Session-based login
* OTP verification for transactions
* User-specific transaction filtering
* Admin and user access separation
* Transaction reference ID generation

---

## 📌 Project Highlights

* Complete online banking workflow
* Multiple transaction systems
* Admin management dashboard
* PDF statement generation
* Clean user interface
* Real-world banking features

---

## 👨‍💻 Author

**Shahrier Shanto**
GitHub: [akira2049](https://github.com/akira2049)

---

## 📜 License

This project is created for academic and learning purposes.
