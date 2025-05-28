# StudentSync

## Overview
StudentSync is a web application designed to help educational institutions manage student records efficiently. Built with Flask, it allows administrators to add, update, delete, and view student information, with user authentication to ensure secure access. The system uses SQLite as its database for storing student data.

## Tech Stack
- **Backend:** Flask (Python)
- **Database:** SQLite (via Flask-SQLAlchemy)
- **Frontend:** HTML, CSS (with Jinja2 templating)
- **Authentication:** Werkzeug for password hashing

## Setup Instructions
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/studentsync.git
   cd studentsync
   ```

2. **Create and Activate a Virtual Environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   The `requirements.txt` file includes:
   ```
   flask==2.0.1
   flask-sqlalchemy==2.5.1
   werkzeug==2.0.1
   ```

4. **Set Up the Database:**
   The app uses SQLite, so no external database setup is required. Run the application to automatically create the database (`students.db`):
   ```bash
   python app.py
   ```

5. **Run the Application:**
   ```bash
   python app.py
   ```
   Open your browser and navigate to `http://127.0.0.1:5000`.

6. **Default Admin Credentials:**
   - Username: `admin`
   - Password: `admin123`
   - Change these credentials after your first login for security.