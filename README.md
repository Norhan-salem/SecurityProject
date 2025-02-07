# Aman - Secure Emailing Service  

![License](https://img.shields.io/badge/license-MIT-blue.svg)  
![FastAPI](https://img.shields.io/badge/backend-FastAPI-green)  
![MongoDB](https://img.shields.io/badge/database-MongoDB-brightgreen)  
![React](https://img.shields.io/badge/frontend-React-blue)  
![Bootstrap](https://img.shields.io/badge/UI-Bootstrap-purple)  

Aman is a **secure emailing service** that ensures a fully encrypted way to send and receive emails while educating users about **network security**. It provides a **step-by-step visual representation** of email encryption, transmission and decryption.  

## ✨ Features  
- **End-to-End Encryption**:  
  - Users can generate **AES keys** or **RSA key pairs** for encryption.  
  - Emails are **AES-encrypted**, and the AES key is encrypted with the recipient's **RSA public key**.  
- **Advanced Security**:  
  - A **challenge-response** authentication pattern ensures that passwords are **never sent over the network**.  
  - **JWT authentication** with **HTTP-only cookies** to prevent **XSS & CSRF attacks**.  
- **Modern & Responsive UI**:  
  - Built with **React.js** and **Bootstrap** for a seamless user experience.  
  - Includes **animations and interactive visuals**.  
- **Secure Database**:  
  - Uses **MongoDB Atlas** to store encrypted email data.  
  - Encryption keys in the database are protected using a **Key Encryption Key (KEK)**.  

---

## 🚀 Installation  

### 1️⃣ Prerequisites  
- **Python 3.x**  
- **FastAPI**  
- **MongoDB Atlas Account**  
- **Node.js & npm (for frontend)**  

### 2️⃣ Clone the Repository  
```sh
git clone https://github.com/Norhan-salem/SecurityProject.git
cd aman

```

### 3️⃣ Backend Setup (FastAPI)

1.  Create and activate a virtual environment:
    
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use: venv\Scripts\activate
    
    ```
    
2.  Install dependencies:
    
    ```sh
    pip install -r requirements.txt
    
    ```
    
3.  Create a **.env** file and add the required environment variables 
(email me @ norhansalem581@gmail.com to get the needed values):
    
    ```ini
    MONGO_URI=mongodb_connection_string
    KEK_SECRET=key_encryption_key
    JWT_SECRET=jwt_secret
    
    ```
    
5.  Start the FastAPI server:
    
    ```sh
    uvicorn main:app --reload
    
    ```
    
    The backend should now be running at **[http://127.0.0.1:8000](http://127.0.0.1:8000/)**.

----------

### 4️⃣ Frontend Setup (React.js + Bootstrap)

1.  Navigate to the frontend directory:
    
    ```sh
    cd frontend/secure-communication-suite
    
    ```
    
2.  Install dependencies:
    
    ```sh
    npm install
    
    ```
    
3.  Start the development server:
    
    ```sh
    npm start
    
    ```
    
    The frontend should now be accessible at **[http://localhost:3000](http://localhost:3000/)**.

----------

## 📌 Usage

1.  **Sign up and log in** using the secure authentication system.
2.  **Generate an AES key** or **RSA key pair** for encryption.
3.  **Compose an email**, encrypt it using AES, and encrypt the AES key with the recipient’s RSA public key.
4.  **Send & Receive emails securely**, with step-by-step visualization of the encryption process.

----------

## 🛠 Contribution

We welcome contributions! Follow these steps:

1.  Fork the repository.
2.  Create a new branch:
    
    ```sh
    git checkout -b feature-name
    
    ```
    
3.  Make your changes and commit them:
    
    ```sh
    git commit -m "Added a new feature"
    
    ```
    
4.  Push to your fork and submit a pull request.

----------

## 🙌 Acknowledgments

-   **FastAPI** for the backend
-   **MongoDB Atlas** for secure cloud storage
-   **JWT & HTTP-only cookies** for authentication
-   **AES & RSA encryption** for email security
-   **React.js & Bootstrap** for frontend development

----------

🚀 **Stay Secure with Aman!**

