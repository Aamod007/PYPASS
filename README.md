# 🔐 **PyPass - Secure Password Manager (Python + MySQL)**  

A secure, terminal-based **Password Manager** developed using **Python** with **MySQL** integration. PyPass encrypts user credentials using **AES-256** and securely stores them in a database, providing a reliable solution to manage multiple passwords effortlessly. The project offers a user-friendly console interface to add, view, update, and delete credentials, ensuring both security and convenience.

---

## 🛠️ **Problem Statement**  
In today's digital world, individuals have numerous accounts across various platforms. Many people tend to use weak or repeated passwords, making their accounts vulnerable to attacks. Password leaks from major websites are common, and reusing passwords across different sites can result in significant security breaches. 

To address this issue, **PyPass** was created as a simple yet powerful tool to help users securely manage their passwords. By using **AES-256 encryption** and **MySQL database integration**, PyPass ensures that sensitive credentials are stored safely and can be accessed only through a master password.

---

## 🧩 **Features**  
- **Secure Storage:** Passwords are encrypted with **AES-256** using a master password.  
- **Clipboard Integration:** Automatically copies retrieved passwords to the clipboard using **pyperclip**.  
- **User-Friendly Console Interface:** Simple terminal-based navigation to manage your credentials.  
- **Database Management:** Utilizes **MySQL** for efficient password storage.  

---

## 📦 **Dependencies**  

Ensure you have the following Python packages installed:  

| Dependency           | Description                                 |
|----------------------|---------------------------------------------|
| [pyperclip](https://pypi.org/project/pyperclip/)        | Clipboard functions for copying passwords. |
| [pycryptodome](https://pypi.org/project/pycryptodome/) | Cryptographic functions for encryption.    |
| [mysql-connector-python](https://pypi.org/project/mysql-connector-python/) | MySQL driver for database operations.       |

---

## 🚀 **Setup**  

Follow these steps to run the project on your system:  

1. **Clone the repository**  
```bash
git clone https://github.com/waterrmalann/PyPass.git
```

2. **Navigate to the project directory and create a virtual environment (optional)**  
```bash
cd PyPass
python -m venv venv
source venv/bin/activate   # For Linux/Mac
venv\Scripts\activate      # For Windows
```

3. **Install the required dependencies**  
```bash
python -m pip install -r requirements.txt
```

4. **Download and install MySQL 8.0**  
[Download MySQL](https://dev.mysql.com/downloads/windows/installer/8.0.html)  

5. **Edit the database credentials in [program.py](program.py)**  
Replace the **'user'** and **'password'** parameters with your MySQL credentials in lines 17-18:  
```python
DATABASE = mysql.connector.connect(
    host="localhost",
    user="your_mysql_username",
    password="your_mysql_password"
)
```

6. **Run the program**  
```bash
python program.py
```

---

## 📸 **Screenshots**  

| **Master Password Prompt** | **Main Menu** |  
|---------------------------|--------------|  
| ![Screenshot](screenshot.png) | ![Screenshot](screenshot.png) |  

---

## ⚠️ **Disclaimer**  

This project was created as a learning tool for password management. **It is not intended for production use** and may contain security vulnerabilities. The encryption functions were implemented quickly and may not follow best practices.  

If you want a more secure and stable password manager, consider using [**pazz**](https://github.com/waterrmalann/pazz), a more refined version of this project that uses **SQLite** and improved security practices.

---

## 📜 **License**  

This project is licensed under **The Unlicense**. See the [LICENSE](LICENSE) file for more details.

---

### 💡 **Note:**  
Feel free to fork this repository, make improvements, and explore more about Python, MySQL, and cryptography.
