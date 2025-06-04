# FLASK_MONGODB_TUTORIAL
This project is a full-stack web application developed using Flask that demonstrates two core functionalities:
Frontend-Backend Separation
Data Handling with MongoDB Atlas and JSON API

🔧 Project Features
Frontend Server (frontend_app.py)
Hosts a form-based interface for users to submit their details (Name, Email, Age, Country). Upon successful submission, the user is redirected to a success.html page. Form data is sent to the backend via a POST request using JavaScript fetch().

Backend Server (backend_app.py)
Handles API requests. It exposes:

POST /submit route: Receives data from the frontend and stores it in MongoDB Atlas.
GET /api route: Reads a data.json file and returns it as a JSON response.

MongoDB Integration
Data submitted from the frontend is inserted securely into a MongoDB Atlas database using the pymongo library.

JSON API
The backend also serves a static JSON list via the /api endpoint, showcasing API response capabilities.
Folder structure
FLASK TUTORIAL-NEW/
│
├── frontend/
│   ├── frontend_app.py
│   ├── templates/
│   │   ├── form.html
│   │   └── success.html
│
├── backend/
│   ├── backend_app.py
│   └── data.json

