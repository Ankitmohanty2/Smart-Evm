# Smart EVM

A smart Ethereum Virtual Machine (EVM) application for managing and interacting with blockchain operations.

## Features

- User authentication and role-based access
- Admin dashboard for management
- Database-driven architecture
- RESTful API endpoints

## Prerequisites

- Python 3.8 or higher ([Download](https://www.python.org/downloads/))
- pip (comes with Python)
- Git
- A code editor (VS Code, Notepad++, etc.)

## Installation

### Step 1: Extract or Clone the Repository

```bash
# If cloning from Git
git clone <repository-url>
cd Smart-Evm

# If you have a zip file, extract it and navigate to the folder
```

### Step 2: Create a Virtual Environment

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Set Up the Database

```bash
python manage.py makemigrations
python manage.py migrate
```

### Step 5: Run the Application

```bash
python manage.py runserver
```

The application will be available at `http://127.0.0.1:8000`

## Usage

### Admin Access

- Navigate to the admin panel at `http://127.0.0.1:8000/admin`
- Log in with your admin credentials
- Manage users, data, and system settings
- Refer to the `info` folder for detailed admin documentation

### User Access

- Create a new account or log in with existing credentials
- Access user dashboard and features
- Refer to the `info` folder for detailed user guide and instructions

## Project Structure

```
Smart-Evm/
├── info/              # Documentation and guides
├── manage.py          # Django management script
├── requirements.txt   # Python dependencies
└── ...
```

## Troubleshooting

**Port already in use?**

If port 8000 is already in use, run the server on a different port:

```bash
python manage.py runserver 8001
```

**Virtual environment not activating?**

Make sure you're in the project directory and try:

```bash
# Windows (PowerShell)
venv\Scripts\Activate.ps1

# Windows (Command Prompt)
venv\Scripts\activate.bat

# macOS/Linux
source venv/bin/activate
```

**Dependencies not installing?**

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

**Database migration errors?**

```bash
python manage.py makemigrations --empty <app_name> --name <migration_name>
python manage.py migrate --fake-initial
```

## Support & Documentation

For more information, please refer to the `info` folder in the project directory.

## License

[Add your license information here]

## Contact & Support

For questions or issues, please open an issue on GitHub or contact the project maintainer.
