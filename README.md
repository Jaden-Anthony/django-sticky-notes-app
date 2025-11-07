# 📝 Django Sticky Notes Task Manager

This is a secure, user-specific task management application built using the Django framework. Users can create, organize, and manage personal notes and tasks, with all data segregated by user for security.

## ✨ Features

* **User Authentication:** Full user lifecycle management (Login, Logout, Registration) using Django's built-in system.
* **Secure CRUD Operations:** Users can Create, Read, Update, and Delete only their own Sticky Notes and Categories.
* **Custom Categories:** Notes can be organized using custom, user-defined categories with unique colors.
* **Styled Forms:** Forms are styled using `django-crispy-forms` and Bootstrap 5 for a clean, user-friendly interface.
* **Testing:** Includes comprehensive unit tests (`notes/tests.py`) covering security, data isolation, and core CRUD use cases.

## 🛠️ Setup and Installation

1.  **Clone the repository:**
    ```bash
    git clone [Your Repository URL Here]
    cd django-sticky-notes-app
    ```

2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Linux/macOS
    venv\Scripts\activate     # On Windows
    ```

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run migrations:**
    ```bash
    python manage.py migrate
    ```

5.  **Create a superuser to access the app and test:**
    ```bash
    python manage.py createsuperuser
    ```

6.  **Run the application:**
    ```bash
    python manage.py runserver
    ```
    Access the application at `http://127.0.0.1:8000/notes/`.

## 🧪 Running Tests

To run the full test suite and confirm all security and CRUD features work correctly:
```bash
python manage.py test notes
