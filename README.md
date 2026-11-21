# Prediction of Inborn Talents Using Fingerprints

## Local setup

Create and activate a Python virtual environment, then install the dependencies:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

Set the required secrets in your shell before running the app. Never commit these
values or a real `.env` file.

```powershell
$env:DJANGO_SECRET_KEY = "generate-a-new-long-random-secret"
$env:EMAIL_HOST_USER = "your-gmail-address@example.com"
$env:EMAIL_HOST_PASSWORD = "your-new-gmail-app-password"
python manage.py runserver
```

Copy `.env.example` as a checklist for the required variable names. The project
does not automatically load `.env` files.
