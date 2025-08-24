# Taskino

Simple Django-based to-do list application.

## Setup

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

The app will be available at http://localhost:8000

## Configuration

`settings.py` reads two environment variables for deployment:

* `DJANGO_ALLOWED_HOSTS` - comma-separated list of allowed hostnames. Defaults to `localhost,127.0.0.1`.
* `DJANGO_CSRF_TRUSTED_ORIGINS` - comma-separated list of full origins (including scheme and port) for CSRF validation. Defaults to local development values like `http://localhost:8000` and `https://localhost:8000`.

If you see a "CSRF verification failed" error when using a different host or port, set `DJANGO_CSRF_TRUSTED_ORIGINS` to include that origin.

## Features
- Create and edit tasks
- Mark tasks as complete
- Categorise tasks (work, study, personal)
