# Milestone 1 – User Authentication System (PolicyNav)

## Description

In this milestone, we developed a secure user authentication system for the PolicyNav application using Streamlit, JWT (JSON Web Tokens), and MongoDB Atlas. The system enables users to create accounts, log in securely, reset forgotten passwords using security questions, and access a protected dashboard after authentication.


## Features Implemented

- User Signup with validation  
- Secure Login using JWT  
- Dashboard after login  
- Forgot Password functionality  
- Password Reset using JWT token and security question
- Ngrok Integration (https://ngrok.com/)
- MongoDB Atlas database integration (https://www.mongodb.com/cloud/atlas) 

## How to Run

1. Install required dependencies  
   ```bash
   pip install streamlit pymongo pyjwt
2. Run the Streamlit application
   ```bash
   streamlit run app.py
3. Use ngrok to expose the application (if required)
   ```bash
   ngrok http 8501

## Screenshots

- Signup Page
  <img width="1918" height="967" alt="image" src="https://github.com/user-attachments/assets/d519ed27-5125-408a-a8c9-936be853d0de" />

- Login Page
  <img width="1918" height="967" alt="image" src="https://github.com/user-attachments/assets/837e98d3-2cf8-47d1-a835-37b93a51e0dd" />

- Dashboard
  <img width="1918" height="965" alt="image" src="https://github.com/user-attachments/assets/3ef2a1e6-6e94-4298-9f3b-a23daee02aec" />

- Forgot Password Page
  <img width="1918" height="966" alt="image" src="https://github.com/user-attachments/assets/39b6cc00-fd11-4851-a5df-3db6145c3656" />
  <img width="1918" height="966" alt="image" src="https://github.com/user-attachments/assets/2c266a68-63d2-48ab-86e9-2286e3863065" />

- Reset Password Page
<img width="1918" height="967" alt="image" src="https://github.com/user-attachments/assets/cb5466b4-df7e-4752-b9d3-59de9b718a39" />

## Notes
- JWT is used for session management and password reset flow.
- MongoDB Atlas is used as the cloud database.

## Author
Arjun L Nair
