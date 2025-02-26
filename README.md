# 🌟 Simple Virtual File System (SVF)

## 📌 Overview
The **Simple Virtual File System (SVF)** is a command-line-based file system written in C++. It supports **user authentication**, **file and directory operations**, and **role-based access control**, making it a lightweight and secure system for managing files.

## 🚀 Features
✅ **User Authentication**: Login system with hashed passwords.  
✅ **Role-Based Access Control**:
   - **Admin**: Full access including user management.
   - **Normal User**: Can create, modify, and delete own files.
   - **Read-Only User**: Can only view files and directories.
✅ **File Operations**: Create, open, read, write, close, delete.  
✅ **Directory Management**: Create, change, list, and remove directories.  
✅ **Permissions Handling**: Enforces security through read/write restrictions.  
✅ **Cross-Platform Support**: Works on **Windows, Linux, and macOS**.  
✅ **Password Security**: SHA-256 hashing for safe storage of credentials.  
✅ **User Persistence**: Stores user credentials in `users.txt` for future logins.  

## 🔧 Prerequisites
- **C++17 or later**
- **OpenSSL** (for password hashing)

### 🛠 Installation
#### **1️⃣ Install Dependencies**
```sh
sudo apt install libssl-dev   # Linux/macOS
```
#### **2️⃣ Compile the Program**
```sh
g++ -o svf SVF.cpp -lssl -lcrypto
```
#### **3️⃣ Run the Program**
```sh
./svf
```

## 📝 Usage Guide
### 1️⃣ **User Management**
```sh
> login <username> <password>       # Log in to the system
> register <username> <password> <role>   # Register new user
> adduser                          # Admin-only user addition
> logout                           # Logout from the system
```

### 2️⃣ **File Operations**
```sh
> touch <filename>   # Create a new file
> open <filename> <mode>   # Open a file (1=Read, 2=Write, 3=Read-Write)
> write <fd> <content>   # Write to an open file
> read <fd>   # Read content from an open file
> close <fd>   # Close an open file
> rm <filename>   # Delete a file
```

### 3️⃣ **Directory Management**
```sh
> mkdir <dirname>   # Create a directory
> cd <dirname>   # Change current directory
> ls [dirname]   # List directory contents
> rmdir <dirname>   # Remove an empty directory
```

### 4️⃣ **Miscellaneous Commands**
```sh
> whoami   # Show current user details
> help   # Show available commands
> exit   # Exit the program
```

## 🎯 Future Enhancements
🔹 Persistent file storage for data retention.  
🔹 Advanced permission management.  
🔹 Enhanced security (two-factor authentication).  
🔹 Logging system to track file system activities.  

## 📜 License
This project is **open-source** and can be freely modified and distributed.  

---
💡 **Developed with C++ | Secure | Lightweight | Role-Based Access**  
🚀 **Enjoy using Simple Virtual File System (SVF)!**

