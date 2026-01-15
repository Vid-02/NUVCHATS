# NUVCHATS

NUVCHATS is an intra-university chat system designed for fast, simple and secure communication among students and faculty. It provides user authentication, private chat rooms, message storage, and a clean browser-based interface. The system is built using PHP, MySQL, JavaScript, and CSS and is suitable for lightweight deployment on any university or internal network server.

---

## Features

### User Authentication
Users are required to log in before entering the chat system. The login logic checks user credentials stored in the database and prevents unauthorized access into the platform.

### Real Time Chat Interface
Inbox style interface that loads messages upon entry into the chat page. Supports interactive message exchange between users who are currently logged in.

### Message Storage
All message history is saved in the MySQL database to allow retrieval of earlier conversations. This ensures persistence even if the browser is refreshed or closed.

### User Listing
The system provides visibility into all registered users of the platform. Users can see who is available and initiate conversations easily.

### Client Side and Server Side Processing
Client side JavaScript manages updates and UI behavior. PHP manages message posting, retrieval, and authentication. SQL scripts handle table creation and storage.

### Lightweight Codebase
Can be deployed on a simple Apache or XAMPP server. Works with minimal system requirements. Suitable for university intranet projects and rapid deployment environments.

---

## Project Structure

```
NUVCHATS/
│
├── img/                       Image assets
├── javascript/                Frontend interactivity scripts
├── php/                       Server side logic and processing
│
├── chat.php                   Main chat room interface
├── chatapp.sql                SQL file containing database schema
├── header.php                 Common UI header component
├── index.php                  Landing page
├── login.php                  Login and authentication page
├── users.php                  User list display
├── style.css                  Styling for UI
├── unzipper.php               Utility script for file extraction
│
└── README.md                  Project documentation
```

---

## Database Setup

Import the `chatapp.sql` file into your MySQL server.  
It contains tables for:

* user credentials  
* chat messages  
* login session details  

Configure database credentials inside the PHP files if required by your deployment environment.

---

## How to Run

### 1. Setup Server Environment
Install any PHP supported web server such as Apache, XAMPP, WAMP, or LAMP.  
Place the NUVCHATS project folder inside the server’s document root.

### 2. Create Database
Create a database and import the `chatapp.sql` file.

### 3. Launch the Application
Open the browser and navigate to:

```
http://localhost/NUVCHATS/index.php
```

Login using available user credentials or update the SQL file to add new accounts.

---

## Technologies Used

* PHP for backend request handling  
* JavaScript for interface behavior and dynamic updates  
* MySQL for storing user and message data  
* HTML and CSS for layout and styling  

---

## Notes

This project was created as a university internal communication tool.  
It can be extended with end-to-end encryption, admin dashboards, private rooms, or notification systems as needed.

