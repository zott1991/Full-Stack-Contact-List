# Flask Backend

This is the backend API for the application, built with Flask.

## Setup

1. Create a virtual environment (already done):
```bash
python -m venv venv
```

2. Activate the virtual environment:
```bash
# Windows PowerShell
.\venv\Scripts\Activate.ps1

# Windows Command Prompt
.\venv\Scripts\activate.bat

# macOS/Linux
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Running the Application

```bash
python app.py
```

The API will be available at `http://localhost:5000`

## API Endpoints

- `GET /` - Welcome message
- `GET /api/health` - Health check endpoint

## Development

The app runs in debug mode by default for development. Remember to disable debug mode in production.


