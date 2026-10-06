# FST_AAT1
Search for new skills

# Skill Exchange Platform

## 📌 Project Title

**Skill Exchange Platform**

## 🎯 Objective

The **Skill Exchange Platform** is a full-stack web application that allows users to share their skills and learn new skills from other users.

The main objective of this project is to create a platform where people can connect with others based on the skills they can **teach** and the skills they want to **learn**.

For example, a user who knows **Python** can teach Python to another user who knows **Graphic Design**, allowing both users to exchange their knowledge.

---

## 📝 Problem Statement

Many students and individuals have useful skills but may not have access to affordable courses or personal mentors.

At the same time, there are many people who are willing to teach their skills but do not have a suitable platform to connect with learners.

The **Skill Exchange Platform** solves this problem by providing a common platform where users can:

* Create their profiles
* Add skills they can teach
* Add skills they want to learn
* Search for other users
* Connect with suitable skill partners
* Exchange knowledge and learn from each other

---

## 🚀 Features

### 👤 User Management

* User registration
* User login
* User profile
* Manage personal skills

### 🧑‍🏫 Skill Management

* Add skills that the user can teach
* Add skills that the user wants to learn
* View available skills

### 🔍 Search

* Search for users based on skills
* Find people who can teach a particular skill

### 🤝 Skill Exchange

* Connect with users having complementary skills
* Send/accept exchange requests
* Exchange knowledge with other users

### 📊 Dashboard

* View personal profile
* View teaching skills
* View learning skills
* View connection/exchange requests

---

## 🛠️ Technologies / Tools Used

### Frontend

* HTML5
* CSS3
* JavaScript
* Bootstrap

### Backend

* Node.js
* Express.js

### Database

* MongoDB

### Development Tools

* Visual Studio Code
* Git
* GitHub
* MongoDB Compass

---

## 🏗️ Project Architecture

```text
Skill Exchange Platform
│
├── Frontend
│   ├── HTML
│   ├── CSS
│   └── JavaScript
│
├── Backend
│   ├── Node.js
│   ├── Express.js
│   ├── Routes
│   └── APIs
│
├── Database
│   └── MongoDB
│
└── GitHub
    └── Source Code & Documentation
```

---

## 📂 Project Structure

```text
skill-exchange-platform/
│
├── public/
│   ├── index.html
│   ├── login.html
│   ├── register.html
│   ├── dashboard.html
│   ├── profile.html
│   ├── skills.html
│   ├── style.css
│   └── script.js
│
├── routes/
│   ├── userRoutes.js
│   └── skillRoutes.js
│
├── models/
│   ├── User.js
│   └── Skill.js
│
├── server.js
├── package.json
├── package-lock.json
└── README.md
```

---

## ⚙️ Installation and Setup

### Step 1: Clone the Repository

Open Command Prompt or VS Code terminal and run:

```bash
git clone YOUR_GITHUB_REPOSITORY_LINK
```

Move into the project folder:

```bash
cd skill-exchange-platform
```

---

### Step 2: Install Dependencies

Run:

```bash
npm install
```

This installs the required Node.js and Express.js packages.

---

### Step 3: Start MongoDB

Make sure MongoDB is installed and running on your computer.

The application uses MongoDB to store:

* User information
* Skills
* Learning preferences
* Teaching preferences
* Exchange requests

---

### Step 4: Start the Server

Run:

```bash
node server.js
```

If the server starts successfully, the terminal will display something similar to:

```text
Server running on http://localhost:3000
MongoDB connected successfully
```

---

### Step 5: Open the Application

Open a browser and visit:

```text
http://localhost:3000
```

The Skill Exchange Platform will be displayed.

---

## 🔄 Working / Methodology

The application works through the following process:

```text
User
  ↓
Registration
  ↓
Login
  ↓
Create Profile
  ↓
Add Teaching Skills
  ↓
Add Learning Skills
  ↓
Search for Users
  ↓
Find Matching Skills
  ↓
Send Exchange Request
  ↓
Accept Request
  ↓
Skill Exchange
```

### Example

Suppose:

**User A**

```text
Can Teach:
Python

Wants to Learn:
Graphic Design
```

**User B**

```text
Can Teach:
Graphic Design

Wants to Learn:
Python
```

The system identifies that their requirements complement each other.

Therefore:

```text
User A  ←→  User B

Python       Graphic Design
```

They can then connect and exchange their knowledge.

---

## 💻 Important Code Snippet

### Express.js Server

```javascript
const express = require("express");

const app = express();

app.use(express.json());
app.use(express.static("public"));

app.get("/", (req, res) => {
    res.sendFile(__dirname + "/public/index.html");
});

app.listen(3000, () => {
    console.log("Server running on http://localhost:3000");
});
```

This code creates the Express.js server and serves the frontend application.

---

## 🗄️ Database

MongoDB is used as the database for storing application data.

Example user document:

```json
{
    "name": "Rahul",
    "email": "rahul@example.com",
    "teachSkills": ["Python", "SQL"],
    "learnSkills": ["Java", "Web Development"]
}
```

---

## 📸 Output

The following screenshots will be included in the GitHub repository and AAT-1 hard-copy report:

### 1. Home Page

*Add screenshot here*

```text
![Home Page](screenshots/home.png)
```

### 2. Registration Page

*Add screenshot here*

```text
![Registration Page](screenshots/register.png)
```

### 3. Login Page

*Add screenshot here*

```text
![Login Page](screenshots/login.png)
```

### 4. User Dashboard

*Add screenshot here*

```text
![Dashboard](screenshots/dashboard.png)
```

### 5. Skill Search

*Add screenshot here*

```text
![Skill Search](screenshots/skill-search.png)
```

### 6. Skill Exchange Request

*Add screenshot here*

```text
![Exchange Request](screenshots/exchange.png)
```

---

## 📁 Screenshots Folder

Screenshots are organized inside:

```text
screenshots/
│
├── home.png
├── register.png
├── login.png
├── dashboard.png
├── skill-search.png
└── exchange.png
```

---

## ⚠️ Challenges Faced

During the development of the project, the following challenges were encountered:

1. Designing a simple and user-friendly interface.
2. Connecting the frontend with the Express.js backend.
3. Connecting the application with MongoDB.
4. Designing the database structure for users and skills.
5. Implementing skill-based user searching.
6. Handling user registration and login.
7. Managing exchange requests between users.
8. Organizing the project files properly.
9. Testing the application and fixing errors.
10. Uploading and maintaining the complete project on GitHub.

---

## 📚 Learning Outcomes

Through this project, the following concepts were learned:

* Development of a full-stack web application.
* HTML, CSS and JavaScript frontend development.
* Node.js and Express.js backend development.
* REST API development.
* MongoDB database management.
* Connecting frontend, backend and database.
* User authentication concepts.
* Git and GitHub repository management.
* Project documentation using Markdown.
* Debugging and testing web applications.
* Organizing and presenting a technical project professionally.

---

## 🔮 Future Enhancements

The project can be improved in the future by adding:

* Real-time chat between users
* Video calling for skill sessions
* Skill ratings and reviews
* Notifications
* AI-based skill recommendations
* Advanced skill matching
* User verification
* Online meeting integration
* Mobile application using Flutter
* Admin dashboard
* Learning progress tracking

---

## 👩‍💻 Project Information

**Project:** Skill Exchange Platform
**Project Type:** Full-Stack Web Application
**Subject:** AAT-1 – Portfolio Driven
**Academic Year:** 2026–2027

---

## 🔗 GitHub Repository

**Repository Link:**


---

## 📄 License

This project is developed for academic and educational purposes.

