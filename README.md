# Django Workspace Setup Guide

Follow these steps to set up and run this Django workspace:

## Prerequisites
- Python 3.x installed
- pip (Python package installer)

## Setup Steps

1. **Clone the repository**
    ```bash
    git clone <repository-url>
    cd sl-3/django
    ```

2. **Create a virtual environment**
    ```bash
    python -m venv venv
    ```

3. **Activate the virtual environment**
    - Windows:
      ```bash
      venv\Scripts\activate
      ```
    - macOS/Linux:
      ```bash
      source venv/bin/activate
      ```

4. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

5. **Apply migrations**
    ```bash
    python manage.py migrate
    ```

6. **Create a superuser (admin)**
    ```bash
    python manage.py createsuperuser
    ```

7. **Run the development server**
    ```bash
    python manage.py runserver
    ```

8. **Access the application**
    - Main site: http://127.0.0.1:8000/
    - Admin interface: http://127.0.0.1:8000/admin/

## Additional Commands

- **Create new app**
  ```bash
  python manage.py startapp app_name
  ```

- **Make migrations after model changes**
  ```bash
  python manage.py makemigrations
  ```

- **Run tests**
  ```bash
  python manage.py test
  ```