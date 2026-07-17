# Django Backend Learning – Day 3

## Project Overview

This project is a beginner-friendly Django backend application created to understand the fundamentals of Django development.
To introduce the intern to Django framework architecture and project structure.

The project demonstrates:

- Creating and configuring a Django project
- Creating a Django app (`core`)
- Understanding Django project structure
- Configuring URL routing
- Building a simple API endpoint using a function-based view
- Running the Django development server

---

## Technologies Used

- Python 3.x
- Django (Latest Stable Version)
- SQLite (Default Django Database)

---

## Project Structure

```text
Day3Django/
│
├── backend/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── core/
│   ├── views.py
│   ├── urls.py
│   ├── models.py
│   ├── admin.py
│   ├── apps.py
│   └── migrations/
│
├── db.sqlite3
├── manage.py
└── venv/
```

---

# Running the Django Project

## 1. Clone the Repository

```bash
git clone <repository-url>
cd Day3Django
```

---

## 2. Create a Virtual Environment (First Time Only)

### Windows

```bash
python -m venv venv
```

### macOS/Linux

```bash
python3 -m venv venv
```

---

## 3. Activate the Virtual Environment

### Windows

```bash
venv\Scripts\activate
```

### macOS/Linux

```bash
source venv/bin/activate
```

---

## 4. Install Dependencies

```bash
pip install django
```

---

## 5. Apply Database Migrations

```bash
python manage.py migrate
```

---

## 6. Start the Development Server

```bash
python manage.py runserver
```

---

## 7. Open in Browser

Visit:

```
http://127.0.0.1:8000/
```

---

# Simple API Endpoint

## Endpoint

```
GET /
```

### Response

```text
Hello Zecpath Backend
```

---

## API Implementation

### `core/views.py`

```python
from django.http import HttpResponse

def home(request):
    return HttpResponse("Hello Zecpath Backend")
```

---

## Test Using Browser

Open:

```
http://127.0.0.1:8000/
```

Expected Output:

```text
Hello Zecpath Backend
```

---

## Test Using curl

```bash
curl http://127.0.0.1:8000/
```

Expected Output:

```text
Hello Zecpath Backend
```

---

## Features

- Django project setup
- Django app configuration
- URL routing
- Function-based view
- Simple text API endpoint
- Beginner-friendly project structure

---

## Author

Created as part of a Django Backend Learning assignment.
