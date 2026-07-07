# Intelligent Freight Quote AI

## Milestone 1 – User Authentication Module

## Project Description

The User Authentication Module is a secure web application developed using Streamlit. It provides user registration, login, password recovery using Security Question and Email OTP, JWT-based session management, and separate dashboards for users and administrators. The application focuses on secure authentication, user validation, and access control.

## Features Implemented

- **User Signup:** Allows new users to register by providing a username, email address, password, security question, and security answer with proper input validation.

- **User Login:** Authenticates registered users using their username/email and password before granting access to the application.

- **Forgot Password (Security Question):** Allows users to securely reset their password by answering the security question selected during registration.

- **Forgot Password (Email OTP):** Sends a One-Time Password (OTP) to the registered email address for secure password verification and password reset.

- **JWT Session Management:** Generates a secure JSON Web Token (JWT) after successful login to maintain the user's authenticated session and restrict unauthorized access.

- **User Dashboard:** Displays a personalized welcome page after successful user authentication.

- **Admin Dashboard:** Provides a separate administrator login to view the list of registered users without displaying password information.

- **Logout Functionality:** Securely ends the user's session by clearing the JWT token and redirecting to the login page.

- **Password Hashing:** Stores passwords and security answers as hashed values to improve security.

- **Input Validation:** Validates mandatory fields, email format, password strength, and confirm password before processing user requests.

## Technologies Used

| Technology |	Purpose |
|------------|----------|
| Python	| Implements the authentication logic and application workflow. |
| Streamlit	| Builds the interactive web application interface. |
| SQLite	| Stores user registration details securely. |
| JWT	| Manages secure user sessions after successful login. |
| bcrypt |	Hashes passwords and security answers before storing them. |
| Gmail | SMTP	Sends OTP emails for password recovery. |
| ngrok	| Generates a public URL to access the application. |
| Google Colab	| Development and execution environment for the project. |

## Colab Secrets Used

| Secret Name	| Purpose |
|-------------|---------|
| JWT_SECRET	| Used to sign and verify JWT session tokens. |
| NGROK_AUTHTOKEN	| Authenticates ngrok to generate a public URL. |
| EMAIL_ADDRESS	| Gmail account used to send OTP emails. |
| EMAIL_PASSWORD |	Gmail App Password used for SMTP authentication. |

## How to Run the Project

1. Open the notebook in Google Colab.
2. Configure the required Colab Secrets.
3. Run all notebook cells.
4. Open the generated ngrok URL.
5. Test the Signup, Login, Forgot Password, User Dashboard, and Admin Dashboard.

## Screenshots

### 1. Login Page

![Login Page](screenshots/login%20page.png)

Allows registered users to securely log in using their username/email and password.


### 2. SignUp Page

![Signup Page](screenshots/signup%20page.png)

Allows new users to create an account by providing the required details.


### 3. Forgot Password (Security Question)

![Forgot Password Security Question](screenshots/forgot%20password%20%28security%20question%29.png)

Allows users to reset their password by verifying their identity through a security question.


