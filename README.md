# Trail Quest
A website where users can browse, review and submit trails.

![trail-quest](https://github.com/user-attachments/assets/4918b5aa-27a6-4d6c-a343-0824f16024e3)

## Brief Documentation

### Creators:

1. GYLLES VARGA 
2. TOMMY TRAN

----  

### Installation and setup instructions.

1.  **Create a virtual environment and activate it**:
```bash
# On Git Bash
## macOS
python3 -m venv .venv
source .venv/bin/activate

## Windows
py -3 -m venv .venv
source .venv/Scripts/activate  
```

2. **Select Python Interpreter in VS Code**:
- Open Command Palette (View > Command Palette or Ctrl+Shift+P)
- Select "Python: Select Interpreter" command
- Choose the virtual environment in your project folder (starts with `./.venv` or `.\.venv`)
![image](https://github.com/user-attachments/assets/2cfa345c-bcc8-4f7c-8f89-4b7de5e9d73c)
- Create a new terminal (Ctrl+Shift+`), automatically activating the virtual environment.

3. **Update pip**:
```bash
python -m pip install --upgrade pip
```

4. **Install requirements**:
```bash
pip install -r requirements.txt
```

5. **Create the database**:
```bash
python manage.py makemigrations
python manage.py migrate
```

6. **Run Server**:
```bash
python manage.py runserver
```
- Ctrl+click the http://127.0.0.1:8000/
----

### Test Files and Instructions

#### 📄 Test File Locations:
All test files are located inside the `trailQuest/tests/` directory:

- `test_models.py` – contains model tests (fields and relationships)
- `test_views.py` – contains view tests for all pages (authenticated and unauthenticated scenarios)
- `test_forms.py` – intended for form tests (to be completed)

#### 🧪 How to Run All Tests:
```bash
python manage.py test
```

### Brief user guide for using the application.
#### 🏠 Landing Page

- home.html is the landing page.
- Accessible at: http://127.0.0.1:8000/
- Shows the navigation bar, server time, search input and all approved trails.

#### 📄 Main web pages and their purpose

| Page                     | Purpose                             |
| ------------------------ | ----------------------------------- |
| `register.html`          | User registration                   |
| `login.html`             | Login for all users                 |
| `profile.html`           | Update preferences and profile info |
| `home.html`              | Explore and search trails           |
| `submit-trail.html`      | Submit a new trail (members only)   |
| `view-trail.html`        | View trail details and reviews      |
| `review-trail.html`      | Submit a trail review and rating    |
| `search-trail-form.html` | Filter/search for trails            |
| `comment.html`           | Leave comments                      |
| `admin-dashboard.html`   | Admin landing page                  |
| `approve-trail.html`     | Admin review/edit/approve trails    |
| `pending-trails.html`    | Admin list of pending trails        |
| `manage-user.html`       | Admin manage user accounts          |
| `review-report.html`     | Admin handle flagged content        |
