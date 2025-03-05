# Blood Donation Management System

## Project Setup Instructions

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)
- Virtual environment (recommended)

### Installation Steps

1. **Extract Project Zip**
   - Unzip the project folder to your desired location

2. **Set Up Virtual Environment**
   ```bash
   # Open command prompt/terminal in project root
   # Create virtual environment
   python -m venv myenv

   # Activate virtual environment
   # Windows:
   myenv\Scripts\activate
   # Mac/Linux:
   source myenv/bin/activate
   ```

3. **Install Dependencies**
   ```bash
   # With virtual environment activated
   pip install django
   ```

4. **Database Setup**
   ```bash
   # Run database migrations
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Create Admin User**
   ```bash
   # Create superuser for admin access
   python manage.py createsuperuser
   # Follow prompts to set username and password
   ```

6. **Run Development Server**
   ```bash
   # Start the server
   python manage.py runserver
   ```

### Accessing the Application
- Main Site: http://127.0.0.1:8000/
- Admin Panel: http://127.0.0.1:8000/admin/

### Troubleshooting
- Ensure virtual environment is activated
- Check Python version (3.8+)
- Verify all dependencies are installed
- If migration issues occur, delete migration files in `bloodgroup_app/migrations/` 
  (except `__init__.py`) and recreate migrations

### Project Features
- Add blood donors
- View donor list
- Track blood group statistics
- Admin management interface

### Requirements
- Python 3.8+
- Django 4.2 or higher

### Deactivating Virtual Environment
```bash
# When done working on the project
deactivate
```

## Note
Always activate the virtual environment before working on the project.
