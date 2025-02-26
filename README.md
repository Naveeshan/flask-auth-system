A simple user authentication system built with Flask, SQLAlchemy, and Flask-WTF. This project allows users to register, log in, and securely store passwords using hashing techniques.
Features:
User Registration with username & password,
Secure Password Hashing using pbkdf2:sha256,
User Login with Authentication,
Form Validation with Flask-WTF,
SQLite Database for storing user details,
Flash Messages for user feedback,
Error Handling & Validation

Tech Stack:
Backend: Flask, SQLAlchemy
Security: Werkzeug (Password Hashing)
Forms: Flask-WTF (WTForms)
Database: SQLite
Frontend: HTML, Jinja2

Project Structure:
/flask-auth-system 
|-- app.py               # Main application file
|-- /templates           
│   |-- home.html        # Homepage
│   |-- register.html    # Registration page
│   |-- login.html       # Login page
|-- /static              # (Optional) Static files like CSS
|-- requirements.txt     # Dependencies
|-- README.md            # Project description

Setup & Installation:

1. Clone the Repository:git clone https://github.com/YOUR_USERNAME/flask-auth-system.git
cd flask-auth-system
2. Create a Virtual Environment:python -m venv venv,
venv\Scripts\activate
3. Install Dependencies:pip install -r requirements.txt
4. Run the Flask App:python app.py
   The app will be running at http://127.0.0.1:5000/

Security Best Practices:
Use environment variables for SECRET_KEY instead of hardcoding it.
Use Flask-Login for session management in future improvements.
Upgrade to PostgreSQL/MySQL for production deployment.

Future Improvements:
Add Flask-Login for better session management.
Implement user roles (admin, regular user).
Integrate JWT-based authentication for API usage.
