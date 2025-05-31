# Email Sender with Flask

![Python](https://img.shields.io/badge/python-3.7+-blue.svg)
![Flask](https://img.shields.io/badge/flask-2.0+-green.svg)
![License](https://img.shields.io/badge/license-MIT-orange.svg)

A simple web application built with Flask that allows users to send emails through a web interface.

## Features

- Send emails with subject and message content
- Responsive web interface
- Form validation
- Success/error feedback
- Easy configuration

## Screenshot

![Email Sender Screenshot](https://i.imgur.com/placeholder.png) *(Replace with actual screenshot)*

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/shivamgarg82/Email-Sender-Flask.git
   cd Email-Sender-Flask
Create and activate a virtual environment (recommended):

bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install dependencies:

bash
pip install -r requirements.txt
Set up environment variables:
Create a .env file in the project root with your email credentials:

EMAIL_USER=your_email@gmail.com
EMAIL_PASSWORD=your_app_specific_password
Configuration
Edit the config.py file to set your preferences:

python
MAIL_SERVER = 'smtp.gmail.com'
MAIL_PORT = 587
MAIL_USE_TLS = True
MAIL_USERNAME = os.environ.get('EMAIL_USER')
MAIL_PASSWORD = os.environ.get('EMAIL_PASSWORD')
Usage
Run the Flask application:

bash
python app.py
Open your web browser and visit:

http://localhost:5000
Fill out the form with recipient email, subject, and message

Click "Send Email"

Security Notes
Never commit your actual email password to version control

For Gmail, use an "App Password" instead of your main password

Consider using environment variables for production deployment

Project Structure
Email-Sender-Flask/
├── app.py                # Main application file
├── config.py             # Email configuration
├── requirements.txt      # Dependencies
├── .env.example          # Environment variables template
├── static/               # Static files (CSS, JS)
│   └── style.css         
├── templates/            # HTML templates
│   ├── base.html         
│   └── index.html        
└── README.md             # This file
Dependencies
Python 3.7+

Flask

Flask-Mail

python-dotenv

Contributing
Contributions are welcome! Please open an issue first to discuss what you'd like to change.

License
MIT


### Additional recommendations:

1. **Add a screenshot**:
   - Replace the placeholder URL with an actual screenshot of your application
   - Recommended tools: Lightshot (Windows) or Flameshot (Linux)

2. **Create a requirements.txt**:
   ```bash
   pip freeze > requirements.txt
Add a .gitignore file with:

venv/
.env
__pycache__/
*.pyc
For better security:

Add instructions for creating Gmail App Passwords

Consider adding rate limiting for production use

Optional enhancements:

Add deployment instructions (Heroku, AWS, etc.)

Include a features roadmap

Add a demo link if deployed online

