---> Registration Management System

A Django-based web application to manage registrations with Create, Read, Update, and Delete (CRUD) functionality. The project uses a MySQL database and includes an interactive user interface built with HTML, CSS, and JavaScript.

---

 ---> Features

- User-friendly interface for managing registrations.
- CRUD operations:
  - **Create**: Add new registration records.
  - **Read**: View all registration records in a table format.
  - **Update**: Edit existing registration records.
  - **Delete**: Remove registration records.
- Form validation on both frontend and backend.
- MySQL database integration for reliable data storage.
- Responsive design for cross-device compatibility.

---

## Installation

### Prerequisites
1. Python (>= 3.9)
2. Django (>= 4.0)
3. MySQL Server
4. MySQL Client for Python (`mysqlclient`)

### Setup Instructions

--->  Clone the repository:

   git clone https://github.com/Adithyashaiva/registration-management-system.git

   test/scripts/activate  ```(for activating virtual environment)```
   
   cd registration-management-system


--->  Configure the database in `settings.py`:
  
   DATABASES = {
       'default': {
           'ENGINE': 'django.db.backends.mysql',
           'NAME': 'your_database_name',
           'USER': 'your_mysql_user',
           'PASSWORD': 'your_mysql_password',
           'HOST': 'localhost',
           'PORT': '3306',
       }
   }


--->  Apply migrations:

   pip install mysqlclient
   python manage.py makemigrations
   python manage.py migrate


--->  Run the server:

   python manage.py runserver


--->  Open the application in your browser:

   http://127.0.0.1:8000/


---

## Usage

- **Create Registration**: Navigate to `/create/`, fill out the form, and submit.
- **View Registrations**: Navigate to the homepage `/` to view all records.
- **Update Registration**: Click the "Edit" button next to a record and update the details.
- **Delete Registration**: Click the "Delete" button next to a record to remove it.

---

## Project Structure

```
registration-management-system/
├── registration/                  # Django project directory
│   ├── settings.py                # Project settings
│   ├── urls.py                    # Project URL configurations
│   ├── wsgi.py                    # WSGI application
├── project/                       # Django app directory
│   ├── models.py                  # Database models
│   ├── views.py                   # Application views
│   ├── forms.py                   # Form validation
│   ├── urls.py                    # App URL configurations
│   ├── templates/                 # HTML templates
│   │   ├── create_registration.html
│   │   ├── view_registrations.html
│   │   ├── update_registration.html
│   │   ├── delete_registration.html
│   ├── static/                    # Static files (CSS, JS)
│       ├── css/
│           ├── create_registration.css
│           ├── view_registrations.css
│           ├── update_registration.css
│           ├── delete_registration.css
├── db.sqlite3                     # SQLite database (if used for development)
├── manage.py                      # Django management script
├── requirements.txt               # Python dependencies
└── README.md                      # Project documentation
```

---

## Technologies Used

- **Backend**: Django Framework
- **Frontend**: HTML, CSS, JavaScript
- **Database**: MySQL
- **Styling**: Unique CSS files for each page
- **Version Control**: Git and GitHub

---

## Author

- Adithya N S - [GitHub Profile](https://github.com/Adithyashaiva)
