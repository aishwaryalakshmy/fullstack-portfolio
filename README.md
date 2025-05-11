# Full-Stack Developer Portfolio

![Portfolio Screenshot](![image](https://github.com/user-attachments/assets/7829c9cc-db75-455d-ab9d-2a7239daf3dc)
) <!-- Replace with your actual screenshot path -->

A responsive personal portfolio website with a fully functional contact form and MySQL backend.

## 🧰 Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript, jQuery  
- **Backend**: PHP, MySQL  
- **Libraries**: SweetAlert2, Typed.js, AOS (Animate On Scroll)

---

## ✨ Features

- 🚀 Modern, animated UI design  
- 📱 Fully responsive on all screen sizes  
- 📬 Contact form with database integration  
- 🗂️ Projects section with descriptions  
- 🧠 Skill icons with interactivity  
- 🧭 Smooth scrolling and progress bar

---

## 🛠️ Installation

### ✅ Prerequisites

- XAMPP / WAMP / MAMP (for local development)  
- PHP 7.0+  
- MySQL 5.7+  
- Modern web browser

### 📥 Setup Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/your-portfolio.git
   cd your-portfolio
````

2. **Import the Database**

   * Open phpMyAdmin
   * Run this SQL:

     ```sql
     CREATE DATABASE portfolio_contact;
     USE portfolio_contact;
     CREATE TABLE messages (
       id INT AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(100) NOT NULL,
       email VARCHAR(100) NOT NULL,
       subject VARCHAR(255) NOT NULL,
       message TEXT NOT NULL,
       created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
     );
     ```

3. **Configure `contact.php`**
   Replace the credentials:

   ```php
   $servername = "localhost";
   $username = "your_db_username";
   $password = "your_db_password";
   $dbname = "portfolio_contact";
   ```

---

## 📁 Project Structure

```
portfolio/
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── script.js
│   └── images/
├── contact.php
├── index.html
├── README.md
└── portfolio_contact.sql
```

---

## 📬 Contact Form (Functionality)

* Sends form input to the MySQL database via AJAX and PHP.
* Uses SweetAlert2 to display success or error messages.

---

## 🌐 Deployment

* Upload files to your hosting server
* Import SQL file into phpMyAdmin
* Ensure `contact.php` is publicly accessible
* Verify PHP and MySQL credentials are correct

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

💖 If you found this helpful, give a ⭐ on GitHub and feel free to fork the project!

```

Let me know if you'd like the actual SQL file (`portfolio_contact.sql`) or help creating a `LICENSE` file too!
```

