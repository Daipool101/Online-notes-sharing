# Online Notes Sharing System - Setup Guide

Follow these steps to set up the project on your local system:

1. **Install Python 3.11 or newer**
   - Download from https://www.python.org/downloads/

2. **Clone or copy the project folder to your local machine**

3. **Open a terminal in the project directory**

4. **Install all required Python libraries**
   - Run:
     ```
     pip install -r requirements.txt
     ```

5. **Run the Flask app**
   - Start the server:
     ```
     python main.py
     ```

6. **Access the website**
   - Open your browser and go to:
     http://127.0.0.1:5000/

7. **Default folders and files**
   - Uploaded documents will be saved in `src/uploads/`
   - Database file will be auto-created as `notes.db` in `src/uploads/`

8. **Troubleshooting**
   - If you change the database model, delete `notes.db` and restart the app.
   - For any errors, check the terminal output for details.

---

**Ready to go!**
