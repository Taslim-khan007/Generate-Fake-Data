# 🚀 Fake User Data Seeder with MySQL & Faker.js

This project automatically generates **100 fake users** and inserts them into a **MySQL database** using **Node.js**, **MySQL2**, and **Faker.js**.

## 📦 Technologies Used
- **Node.js** 🟢
- **Express.js** ⚡ (optional for server handling)
- **MySQL** 🗄️
- **MySQL2** npm package
- **Faker.js** 🎭 for fake data generation

## 🛠️ Installation Steps
1️⃣Clone the repository**
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
2️⃣ Install dependencies
npm install express mysql2 @faker-js/faker
3️⃣ Setup MySQL Database
CREATE DATABASE delta_app;
USE delta_app;

CREATE TABLE user (
  id VARCHAR(36) PRIMARY KEY,
  email VARCHAR(100),
  username VARCHAR(50),
  password VARCHAR(100)
);
4️⃣ Update Database Credentials
Edit index.js:

const connection = mysql.createConnection({
  host: 'localhost',
  user: 'root',
  database: 'delta_app',
  password: 'your_password'
});
5️⃣ Run the Script
node index.js

## 📜 How It Works
Uses Faker.js to create:
🆔 Random UUID
👤 Username
📧 Email
🔑 Password
Inserts 100 fake users into the MySQL database at once.

