# Little Lemon Web Application

## Table of Contents
1. [About the Project](#about-the-project)
2. [Features](#features)
3. [API Endpoints](#api-endpoints)
4. [Installation Instructions](#installation-instructions)
5. [Usage](#usage)
6. [Peer Review Instructions](#peer-review-instructions)
7. [Grading Criteria](#grading-criteria)
8. [Good Luck!](#good-luck)

---

## About the Project
This project is part of the **final graded assessment** for the back-end development course. It demonstrates the use of **Django** and the **Django REST Framework** to create a web application for the Little Lemon restaurant. The application focuses on handling table bookings through a **REST API** integrated with a **MySQL database**.

The primary goals of this project are to:
- **Connect the Django back-end to MySQL**.
- **Set up a table booking API**.
- **Insert and retrieve booking data via the API**.
- **Implement dynamic front-end functionality using JavaScript**.

---

## Features
- **Static HTML Content**: The application serves static HTML templates using Django.
- **Menu and Booking APIs**: Two endpoints are implemented for managing menu items and table bookings.
- **User Registration and Authentication**: Basic user authentication is included.
- **Database Integration**: MySQL is used as the database for storing bookings and menu data.
- **Unit Tests**: The application includes unit tests to ensure API functionality.
- **API Testing**: The APIs can be tested using the **Insomnia REST Client** or similar tools.
- **Dynamic Front-End**: JavaScript is used to dynamically update the booking interface based on available slots and user input.

---

## API Endpoints
Here are the primary API paths that can be tested:

| Endpoint                 | Method | Description                          |
|--------------------------|--------|--------------------------------------|
| `/api/bookings/`         | GET    | Retrieves all bookings for a specific date. |
| `/api/bookings/`         | POST   | Creates a new booking.               |
| `/api/menu/`             | GET    | Retrieves all menu items.            |
| `/api/menu/`             | POST   | Adds a new menu item (authentication required). |
| `/api/registration/`     | POST   | Registers a new user.                |
| `/api/login/`            | POST   | Authenticates a user.                |
| `/api/logout/`           | POST   | Logs out the current user.           |

---

## Installation Instructions
### Prerequisites
- **Python 3.9+**
- **Django 4.x**
- **MySQL 8.0+**
- **VS Code Editor**
- **pipenv**

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/Cod-e-Codes/littlelemon
   cd littlelemon
   ```
2. Activate the virtual environment:
   ```bash
   pipenv shell
   ```
3. Install dependencies:
   ```bash
   pipenv install
   ```
4. Configure MySQL database:
   - Create a MySQL database named `reservations`.
   - Update the `DATABASES` configuration in `settings.py` with your MySQL credentials.
5. Perform database migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
6. Run the development server:
   ```bash
   python manage.py runserver
   ```

---

## Usage
### Testing the Application
- **Access the Web Interface**: Navigate to `http://127.0.0.1:8000/` to interact with the restaurant’s booking and menu system.
- **Test APIs**:
  - Use tools like **Insomnia** or **Postman** to test the API endpoints listed above.

### Unit Tests
Run the unit tests to verify functionality:
```bash
python manage.py test
```

---

## Peer Review Instructions
1. **Project Submission**:
   - Ensure all code changes are committed and pushed to the GitHub repository.
   - Include this `README.md` file with API paths and instructions.
2. **Submission Steps**:
   - Go to the submission portal and provide a title, e.g., *Back-end Developer Capstone Project*.
   - Paste the GitHub repository URL.
   - Preview and submit your project.

---

## Grading Criteria
- **Static HTML Content**: Does the application use Django to serve static HTML templates?
- **Git Repository**: Is the project committed to a GitHub repository?
- **Database Connection**: Is the backend successfully connected to MySQL?
- **API Implementation**: Are the menu and booking APIs functional?
- **Authentication**: Does the application implement user registration and authentication?
- **Unit Tests**: Are unit tests present and functional?
- **API Testing**: Can the APIs be tested with Insomnia?

---

## Good Luck!
Thank you for reviewing this project. If you have any questions or feedback, feel free to reach out!

