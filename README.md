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

## Features
- Create and edit tasks
- Mark tasks as complete
- Categorise tasks (work, study, personal)
