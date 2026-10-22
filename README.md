# Insurance Management System 🛡️

A Django-based Insurance Management System that allows admins to manage insurance policies and customers to apply for policies online.

## Features

### Admin
- Login / Logout
- Manage Insurance Categories (Add, Update, Delete)
- Manage Insurance Policies (Add, Update, Delete)
- View all Customers
- Approve / Disapprove Policy Applications
- Reply to Customer Questions

### Customer
- Register / Login
- View available Policies
- Apply for a Policy
- View Application History
- Ask Questions to Admin

## Tech Stack

- **Backend**: Python, Django 6.x
- **Database**: SQLite3
- **Frontend**: HTML, CSS, Bootstrap
- **Libraries**: django-widget-tweaks, Pillow

## Setup Instructions

```bash
# 1. Clone the repository
git clone https://github.com/Bhuvankarthik06/insurance-management.git
cd insurance-management

# 2. Create a virtual environment
python -m venv venv
venv\Scripts\activate   # Windows
# source venv/bin/activate  # Linux/Mac

# 3. Install dependencies
pip install django django-widget-tweaks pillow

# 4. Run migrations
python manage.py migrate

# 5. Create a superuser (admin)
python manage.py createsuperuser

# 6. Run the development server
python manage.py runserver
```

Open your browser and navigate to: **http://127.0.0.1:8000**

## Pages

| URL | Description |
|-----|-------------|
| `/` | Home Page |
| `/adminlogin` | Admin Login |
| `/customersignup` | Customer Registration |
| `/admin` | Django Admin Panel |

## License

This project is open source and available under the [MIT License](LICENSE).
