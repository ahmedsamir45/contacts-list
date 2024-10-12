# Contact Manager

This project is a simple Contact Manager application with a React frontend and a Flask backend. It allows users to create, read, update, and delete contact information.

## Features

- View a list of contacts
- Create new contacts
- Edit existing contacts
- Delete contacts

## Tech Stack

### Frontend
- React
- CSS

### Backend
- Flask
- SQLAlchemy

## Project Structure

```
contact-manager/
├── frontend/
│   ├── src/
│   │   ├── App.js
│   │   ├── ContactList.js
│   │   ├── ContactForm.js
│   │   └── App.css
│   └── ...
├── backend/
│   ├── app.py
│   ├── config.py
│   └── models.py
└── README.md
```

## Setup and Installation

### Frontend

1. Navigate to the `frontend` directory
2. Install dependencies:
   ```
   npm install
   ```
3. Start the development server:
   ```
   npm start
   ```

### Backend

1. Navigate to the `backend` directory
2. Create a virtual environment:
   ```
   python -m venv venv
   ```
3. Activate the virtual environment:
   - On Windows: `venv\Scripts\activate`
   - On macOS and Linux: `source venv/bin/activate`
4. Install dependencies:
   ```
   pip install flask flask-sqlalchemy
   ```
5. Run the Flask application:
   ```
   python app.py
   ```

## API Endpoints

- `GET /contacts`: Retrieve all contacts
- `POST /create_contact`: Create a new contact
- `PATCH /update_contact/<int:user_id>`: Update an existing contact
- `DELETE /delete_contact/<int:user_id>`: Delete a contact

## Data Model

The `Contact` model includes the following fields:
- `id`: Integer (Primary Key)
- `first_name`: String
- `last_name`: String
- `email`: String

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).
