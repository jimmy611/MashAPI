# MashAPI
An autorization API for login and registern using Django rest framework and simple jwt token
# MashAPI - Django REST Framework API with Authorization

## Overview
MashAPI is a Django REST Framework API that provides user registration and login functionality using Simple JWT for token-based authentication.

## Requirements
- Python 3.x
- Django
- Django REST Framework
- djangorestframework-simplejwt

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/jimmy611/MashAPI.git
   cd MashAPI

#optional
python -m venv venv
source venv/bin/activate  # On Windows, use 'venv\Scripts\activate'

#Install dependencies:
pip install -r requirements.txt

#Apply database migrations:
python manage.py migrate

python manage.py runserver


Endpoints
User Registration
URL: /api/register/
Method: POST
Request Body:
json
Copy code
{
    "username": "your_username",
    "email": "your_email@example.com",
    "password": "your_password"
}

User Login
URL: /api/login/
Method: POST
Request Body:
json
Copy code
{
    "username": "your_username",
    "password": "your_password"
}
Response:
json
Copy code
{
    "access": "your_access_token",
    "refresh": "your_refresh_token"
}


