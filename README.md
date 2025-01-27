
# Django User Authentication Application

## Overview
This is a Django-based web application that includes user authentication features such as sign-up, login, password management, and restricted pages for logged-in users. The app provides a clean and simple interface to handle user accounts.

# Bootstrap
Use Bootstrap for formating the templates.

## Features
- **Sign Up**: 
  - Users can register with a username, email, and password.
  - Automatic login after successful registration.

- **Login**:
  - Allows users to log in using their username or email and password.

- **Forgot Password**:
  - Users can request a password reset via email.

- **Change Password**:
  - Authenticated users can update their password.

- **Dashboard**:
  - Restricted to logged-in users. Displays a greeting and links to profile and logout.

- **Profile**:
  - Shows user details (username, email, date joined, etc.). Restricted to logged-in users.

- **Logout**:
  - Logs the user out and redirects to the homepage.

## Application Flow
1. **Homepage**:
   - Accessible to everyone.
2. **Authentication Pages**:
   - Sign Up, Login, and Forgot Password.
3. **Restricted Pages**:
   - Dashboard and Profile (only accessible to authenticated users).

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <project-directory>
   ```
2. Install dependencies:
   ```bash
   rm -rf venv
   python3 -m venv venv
   source venv/bin/activate
   pip install django
   ```
4. Apply migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
5. Start the development server:
   ```bash
   python manage.py runserver
   ```
6. Access the app at `http://127.0.0.1:8000/`.

## Configuration
- **Database**: SQLite3 is used as the default database.
- **Email Backend**: Emails are printed to the console for testing purposes. Update the `EMAIL_BACKEND` in `settings.py` for production.


## Dependencies
- Django (5.1.5)


