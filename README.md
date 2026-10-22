# Insurance Management System - Deployment Guide

## Live Demo
> ?? **Deployed on Railway**: Will be updated after deployment

## Quick Start (Local Development)
`ash
git clone https://github.com/Bhuvankarthik06/insurance-management.git
cd insurance-management
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
`
Open: http://127.0.0.1:8000

## Deploy to Railway

1. Go to [railway.app](https://railway.app) and sign in with GitHub
2. Click **New Project** ? **Deploy from GitHub repo**
3. Select Bhuvankarthik06/insurance-management
4. Railway will auto-detect and deploy using ailway.toml
5. Set these environment variables in Railway dashboard:
   - SECRET_KEY = (generate a secure random key)
   - DEBUG = False
6. Click **Deploy** — your live URL will be shown in the dashboard

## Environment Variables (Railway Dashboard)

| Variable | Value |
|----------|-------|
| SECRET_KEY | Your secure secret key |
| DEBUG | False |

## Tech Stack
- **Backend**: Python 3.11, Django 6.x
- **Database**: SQLite3 (local) / Configurable via DATABASE_URL
- **Frontend**: HTML, CSS, Bootstrap
- **Static Files**: WhiteNoise
- **Server**: Gunicorn

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

## Pages

| URL | Description |
|-----|-------------|
| / | Home Page |
| /adminlogin | Admin Login |
| /customersignup | Customer Registration |
| /admin | Django Admin Panel |

## License
This project is open source and available under the [MIT License](LICENSE).
