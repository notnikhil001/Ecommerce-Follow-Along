# Milestone 7 - User Login Authentication Backend

## 🚀 Overview
In this milestone, we implemented a backend endpoint for user login. The focus was on validating user credentials, securely comparing encrypted passwords, and ensuring authentication.

## 🎯 Learning Goals
By completing this milestone, we:
- Understood how to validate user credentials during login.
- Learned how to compare the encrypted password with the user’s input.
- Strengthened security by using password hashing.

## 🔑 How Login Authentication Works
1. **User Enters Credentials**
   - The user provides their email/username and password on the login page.
2. **Fetch User Data from Database**
   - The backend retrieves the user record based on the provided email/username.
   - If the user is not found, an error message is returned: *"User does not exist."*
3. **Compare Encrypted Passwords**
   - The entered password is hashed using `bcrypt`.
   - The resulting hash is compared with the stored hashed password.
   - If they match, the user is authenticated; otherwise, an error is sent.

## 📝 Steps Implemented
### 1️⃣ Create Login Endpoint
- Accepts user credentials (`email/username` and `password`).
- Retrieves the corresponding user from the database.

### 2️⃣ Validate Password
- Uses `bcrypt.compare()` to securely check if the entered password matches the stored hashed password.
- If authentication is successful, a success response is returned.
- If authentication fails, an appropriate error message is returned.

## 🛠️ Technologies Used
- **Node.js** - Backend runtime environment.
- **Express.js** - Web framework for building APIs.
- **MongoDB** - Database for storing user information.
- **Mongoose** - ODM for MongoDB.
- **bcrypt.js** - Library for password hashing and comparison.

## 📥 Submission Guidelines
- **Code Push:** Committed and pushed all changes to the GitHub repository.
- **Public Repository:** Ensured the repository is publicly accessible.
- **README Update:** This document summarizes our login functionality progress.
- **Submission:** Shared the GitHub repository link in the assignment submission section.


## 📌 How to Run the Project
1. Clone the repository:
   ```sh
   git clone <repository-link>
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Set up `.env` file with the following variables:
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   ```
4. Start the server:
   ```sh
   npm start
   ```

