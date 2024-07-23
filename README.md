# G-Notify Backend

## Introduction
Goma-Notify is a comprehensive vehicle document renewal system designed to streamline the renewal process for vehicle owners in Ethiopia. This Django backend serves as the core of the system, managing user data, notifications, and service integrations.

## Features
- **User Registration and Profile Management**: Secure and efficient handling of user data.
- **Deadline Notifications**: Sends timely reminders via email and in-app alerts to ensure users do not miss renewal deadlines.
- **Document Renewal Services**: Facilitates the renewal of various vehicle documents.
- **Map System**: Helps users locate bolo inspection providers.
- **Digital Payment System**: Integrates with Chapa for seamless digital payments.

## Installation

### Prerequisites
- Python 3.8+
- Django 3.2+
- PostgreSQL

### Steps

#### Clone the repository:
```bash
git clone https://github.com/solo21-12/g-notifu-registration.git 
cd g-notifu-registration
```

#### Create and activate a virtual environment:
```bash
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
```

#### Install the required dependencies:
```bash
pip install -r requirements.txt
```

#### Set up the database:
- Create a PostgreSQL database for the project.
- Update the `DATABASES` setting in `settings.py` with your database details.

#### Apply migrations:
```bash
python manage.py migrate
```

#### Create a superuser:
```bash
python manage.py createsuperuser
```

#### Run the development server:
```bash
python manage.py runserver
```

## Usage
- Access the admin panel at `http://127.0.0.1:8000/admin/` to manage users and other data.
- Use the API endpoints to interact with the backend from the Flutter frontend.

## Contributors
- Fita Wegene
- Dawit Abraham
- Daniel Yirdaw
- Addis Seteye

## Frontend Repository
For the Flutter frontend of this project, refer to the [G-Notify](https://github.com/belteshazzer/Goma).
