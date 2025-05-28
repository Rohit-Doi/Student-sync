<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>StudentSync README</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 40px; line-height: 1.6; }
        h1, h2, h3 { color: #333; }
        pre { background: #f4f4f4; padding: 10px; border-radius: 5px; }
        code { font-family: monospace; }
    </style>
</head>
<body>
    <h1>StudentSync</h1>

    <h2>Overview</h2>
    <p>StudentSync is a web application designed to help educational institutions manage student records efficiently. Built with Flask, it allows administrators to add, update, delete, and view student information, with user authentication to ensure secure access. The system uses SQLite as its database for storing student data.</p>

    <h2>Features</h2>
    <ul>
        <li><strong>User Authentication:</strong> Secure login for administrators to access the system.</li>
        <li><strong>Student CRUD Operations:</strong>
            <ul>
                <li>Add new students with details like name, roll number, class, and contact information.</li>
                <li>View a list of all students.</li>
                <li>Update existing student records.</li>
                <li>Delete student records.</li>
            </ul>
        </li>
        <li><strong>Database Storage:</strong> Uses SQLite to store student data persistently.</li>
        <li><strong>Responsive Design:</strong> Basic CSS styling for a user-friendly interface.</li>
    </ul>

    <h2>Tech Stack</h2>
    <ul>
        <li><strong>Backend:</strong> Flask (Python)</li>
        <li><strong>Database:</strong> SQLite (via Flask-SQLAlchemy)</li>
        <li><strong>Frontend:</strong> HTML, CSS (with Jinja2 templating)</li>
        <li><strong>Authentication:</strong> Werkzeug for password hashing</li>
    </ul>

    <h2>Prerequisites</h2>
    <ul>
        <li>Python 3.8 or higher</li>
        <li>Git (for cloning the repository)</li>
        <li>A virtual environment tool (e.g., <code>venv</code>)</li>
    </ul>

    <h2>Setup Instructions</h2>
    <ol>
        <li><strong>Clone the Repository:</strong>
            <pre><code>git clone https://github.com/yourusername/studentsync.git
cd studentsync</code></pre>
        </li>
        <li><strong>Create and Activate a Virtual Environment:</strong>
            <pre><code>python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate</code></pre>
        </li>
        <li><strong>Install Dependencies:</strong>
            <pre><code>pip install -r requirements.txt</code></pre>
            <p>The <code>requirements.txt</code> file includes:</p>
            <pre><code>flask==2.0.1
flask-sqlalchemy==2.5.1
werkzeug==2.0.1</code></pre>
        </li>
        <li><strong>Set Up the Database:</strong>
            <p>The app uses SQLite, so no external database setup is required. Run the application to automatically create the database (<code>students.db</code>):</p>
            <pre><code>python app.py</code></pre>
        </li>
        <li><strong>Run the Application:</strong>
            <pre><code>python app.py</code></pre>
            <p>Open your browser and navigate to <code>http://127.0.0.1:5000</code>.</p>
        </li>
        <li><strong>Default Admin Credentials:</strong>
            <ul>
                <li>Username: <code>admin</code></li>
                <li>Password: <code>admin123</code></li>
                <li>Change these credentials after your first login for security.</li>
            </ul>
        </li>
    </ol>

    <h2>Project Structure</h2>
    <pre><code>studentsync/
├── app.py                # Main Flask application
├── models.py             # Database models (Student, User)
├── templates/            # HTML templates
│   ├── base.html
│   ├── index.html
│   ├── login.html
│   ├── add_student.html
│   ├── view_students.html
│   ├── update_student.html
├── static/               # Static files (CSS, JS, images)
│   ├── css/
│   │   └── styles.css
│   ├── js/
│   │   └── scripts.js
├── requirements.txt      # Python dependencies
└── students.db           # SQLite database (created on first run)
</code></pre>

    <h2>Usage</h2>
    <ol>
        <li><strong>Log In:</strong>
            <p>Navigate to <code>/login</code> and use the default admin credentials.</p>
        </li>
        <li><strong>Add a Student:</strong>
            <p>Go to <code>/add_student</code> to enter student details.</p>
        </li>
        <li><strong>View Students:</strong>
            <p>Visit <code>/view_students</code> to see a list of all students.</p>
        </li>
        <li><strong>Update/Delete Students:</strong>
            <p>From the student list, click on a student to update or delete their record.</p>
        </li>
    </ol>

    <h2>Contributing</h2>
    <p>Contributions are welcome! To contribute:</p>
    <ol>
        <li>Fork the repository.</li>
        <li>Create a new branch (<code>git checkout -b feature/your-feature</code>).</li>
        <li>Make your changes and commit (<code>git commit -m "Add your feature"</code>).</li>
        <li>Push to your branch (<code>git push origin feature/your-feature</code>).</li>
        <li>Open a Pull Request.</li>
    </ol>

    <h2>License</h2>
    <p>This project is licensed under the MIT License. See the <a href="LICENSE">LICENSE</a> file for details.</p>

    <h2>Contact</h2>
    <p>For any questions or issues, please open an issue on GitHub or contact [your email].</p>
</body>
</html>
