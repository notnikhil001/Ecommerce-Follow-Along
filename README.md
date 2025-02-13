🚀 Milestone 6: Secure User Signup with Password Encryption

📌 Overview
In this milestone, we built a backend endpoint for user signup, ensuring secure password storage using bcrypt.

🔐 Key Features
Password Encryption: User passwords are hashed before saving to the database.
Secure Data Storage: User details (name, email, etc.) are stored safely with encrypted passwords.
🛠️ Technologies Used
Node.js
Express.js
MongoDB
bcrypt.js
📂 How to Run
Clone the repository
Install dependencies: npm install
Start the server: npm start
📌 API Endpoint
POST /signup

Request Body:
{
  "name": "John Doe",
  "email": "johndoe@example.com",
  "password": "securepassword"
}
Response:
{
  "message": "User registered successfully!"
}
