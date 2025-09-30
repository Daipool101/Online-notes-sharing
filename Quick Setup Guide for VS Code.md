# Quick Setup Guide for VS Code

This guide provides step-by-step instructions to quickly set up and run the Online Notes Sharing System in Visual Studio Code.

## Prerequisites

- Python 3.8 or higher
- Visual Studio Code
- Git (optional)

## Quick Setup Steps

### 1. Open Project in VS Code

1. Download and extract the project files
2. Open VS Code
3. Go to `File > Open Folder`
4. Select the `online_notes_sharing_system` folder

### 2. Open Terminal in VS Code

1. Press `Ctrl+`` (backtick) or go to `Terminal > New Terminal`
2. Navigate to the backend directory:
   ```bash
   cd backend/notes_sharing_backend
   ```

### 3. Set Up Python Environment

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install flask flask-sqlalchemy flask-cors werkzeug
```

### 4. Create Required Directories

```bash
# Create uploads directory
mkdir -p src/uploads
```

### 5. Run the Application

```bash
python src/main.py
```

### 6. Access the Application

Open your web browser and go to: `http://localhost:5000`

## Default Login Credentials

- **Admin Username**: `admin`
- **Admin Password**: `admin123`

## VS Code Extensions (Recommended)

Install these extensions for better development experience:

1. **Python** - Python language support
2. **Pylance** - Python language server
3. **Flask Snippets** - Flask code snippets
4. **Live Server** - Live reload for frontend development

## Quick Test

1. Register a new user account
2. Login with the new account
3. Upload a test file (PDF, DOC, etc.)
4. Login as admin and approve the file
5. Browse and download the approved file

## Troubleshooting

### Common Issues:

1. **Port already in use**: Change port in `src/main.py` from 5000 to another port
2. **Permission errors**: Run terminal as administrator (Windows) or use `sudo` (macOS/Linux)
3. **Module not found**: Ensure virtual environment is activated and dependencies are installed

### Need Help?

Refer to the complete `README.md` file for detailed documentation and troubleshooting guide.

## Project Structure

```
online_notes_sharing_system/
├── README.md                    # Complete documentation
├── SETUP_GUIDE.md              # This quick setup guide
└── backend/
    └── notes_sharing_backend/
        ├── venv/                # Virtual environment
        ├── requirements.txt     # Dependencies
        └── src/
            ├── main.py         # Run this file
            ├── static/         # Web interface
            ├── models/         # Database models
            ├── routes/         # API endpoints
            └── uploads/        # Uploaded files
```

## Next Steps

After successful setup:

1. Read the complete `README.md` for full feature documentation
2. Explore the admin panel functionality
3. Test file upload and download features
4. Customize the application as needed

Happy coding! 🚀

