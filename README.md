# Full-Stack Contact List Application

A modern, full-stack contact management application built with Flask (Python) backend and React (Vite) frontend.

## Features

- ✨ Create, Read, Update, and Delete (CRUD) contacts
- 🎨 Beautiful, responsive UI with modal forms
- 🔄 Real-time updates
- 🗄️ SQLite database
- 🌐 RESTful API architecture

## Tech Stack

### Backend
- **Flask** - Python web framework
- **Flask-SQLAlchemy** - ORM for database operations
- **Flask-CORS** - Cross-Origin Resource Sharing support
- **SQLite** - Lightweight database

### Frontend
- **React** - UI library
- **Vite** - Fast build tool and dev server
- **Modern CSS** - Custom styling with animations

## Project Structure

```
Py_Java_App/
├── backend/
│   ├── app.py           # Flask app initialization
│   ├── config.py        # Database and app configuration
│   ├── main.py          # API routes and server
│   ├── models.py        # Database models
│   ├── requirements.txt # Python dependencies
│   └── instance/        # SQLite database location
│
├── frontend/
│   ├── src/
│   │   ├── App.jsx          # Main application component
│   │   ├── ContactList.jsx  # Contact list display
│   │   ├── ContactForm.jsx  # Form for create/update
│   │   └── App.css          # Styles
│   ├── package.json     # Node dependencies
│   └── vite.config.js   # Vite configuration
│
└── README.md
```

## Installation & Setup

### Prerequisites
- Python 3.8+
- Node.js 16+
- npm or yarn

### Backend Setup

1. Navigate to the backend directory:
```bash
cd backend
```

2. Create and activate a virtual environment:
```bash
# Windows
python -m venv venv
.\venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run the Flask server:
```bash
python main.py
```

The backend will run on `http://localhost:5000`

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

The frontend will run on `http://localhost:5173` (or another port if 5173 is busy)

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/contacts` | Get all contacts |
| POST | `/create_contact` | Create a new contact |
| PATCH | `/update_contact/<id>` | Update a contact by ID |
| DELETE | `/delete_contact/<id>` | Delete a contact by ID |

### Request Body Format

```json
{
  "firstName": "John",
  "lastName": "Doe",
  "email": "john.doe@example.com"
}
```

## Usage

1. Start both the backend and frontend servers (follow installation steps above)
2. Open your browser to the frontend URL (usually `http://localhost:5173`)
3. Use the interface to:
   - View all contacts in the table
   - Click "Create New Contact" to add a new contact
   - Click "Update" to edit an existing contact
   - Click "Delete" to remove a contact

## Features in Detail

### Contact Management
- **Create**: Click the "Create New Contact" button to open a modal form
- **Read**: All contacts are displayed in a table on the main page
- **Update**: Click "Update" on any contact to edit their information
- **Delete**: Click "Delete" to remove a contact (with confirmation)

### Responsive Design
- Clean, modern interface
- Smooth animations and transitions
- Mobile-friendly layout

## Database Schema

### Contact Model
```python
{
  id: Integer (Primary Key)
  first_name: String(100) - Required
  last_name: String(100) - Required
  email: String(100) - Required, Unique
}
```

## Development

### Backend Development
The Flask server runs with debug mode enabled for development. Changes to Python files will automatically reload the server.

### Frontend Development
Vite provides hot module replacement (HMR), so changes to React components will instantly reflect in the browser.

## Future Enhancements

- [ ] User authentication and authorization
- [ ] Search and filter functionality
- [ ] Pagination for large contact lists
- [ ] Export contacts to CSV
- [ ] Contact groups/categories
- [ ] Phone number field
- [ ] Address information
- [ ] Profile pictures

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Author

**zott1991**

- GitHub: [@zott1991](https://github.com/zott1991)
- Repository: [Full-Stack-Contact-List](https://github.com/zott1991/Full-Stack-Contact-List)

## Acknowledgments

- Flask documentation
- React documentation
- Vite documentation

---

⭐ If you found this project helpful, please give it a star!

