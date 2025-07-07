# PLANIVA Event Management Platform

## Overview
PLANIVA is an event management platform that combines AI and human expertise to help users plan, organize, and manage events such as weddings, college fests, and other special occasions. The platform offers a seamless experience for both event organizers and vendors, providing a wide range of services including catering, decor, venues, sound, lighting, attire, photography, videography, and more.

## Features
- User registration and authentication
- Dashboard for managing event plans
- Browse and select from a variety of event services
- Vendor management and consultation
- Add event plans to cart
- View and manage ongoing, past, and upcoming events
- Responsive frontend with modern UI
- Backend API built with Flask and SQLite

## Folder Structure
```
├── ABOUT PAGE.html           # About Planiva
├── Attire.html               # Attire vendor page
├── BBQ.html                  # Catering vendor page
├── Caterer.html              # Catering services
├── Contact.html              # Contact information
├── Creatives.html            # Creative services
├── dashboard.css             # Dashboard styles
├── Database (1).db           # SQLite database
├── Decor.html                # Decor vendor page
├── Frontend.html             # Main landing page
├── Hotels.html               # Hotel vendor page
├── JavScript.js              # (Empty/placeholder)
├── JS CHALLENGE.html         # (Unrelated challenge page)
├── Lighting.html             # Lighting vendor page
├── Makeup.html               # Makeup vendor page
├── NEW EVENT.html            # Event planning form
├── Photography.html          # Photography vendor page
├── Register.html             # User registration page
├── Rentals.html              # Rentals vendor page
├── Services Offered.html     # List of services
├── Services.html             # Main services page
├── Sign In Page.html         # User sign-in page
├── Sound.html                # Sound vendor page
├── style.css                 # Main styles
├── style1.css                # Additional styles
├── Testimonials.html         # Customer testimonials
├── User Dashboard.html       # User dashboard
├── Userflows (1).py          # Flask backend API
├── Venues.html               # Venues vendor page
├── Videography.html          # Videography vendor page
```

## Setup Instructions

### Prerequisites
- Python 3.x
- pip (Python package manager)
- Flask (`pip install flask`)
- Flask-CORS (`pip install flask-cors`)
- SQLite3 (comes with Python standard library)

### 1. Clone the Repository
```
git clone <repo-url>
cd <repo-folder>
```

### 2. Install Python Dependencies
```
pip install flask flask-cors
```

### 3. Database Setup
- The project uses an SQLite database file: `Database (1).db`.
- Ensure this file is present in the project root. If you need to initialize a new database, create the required tables as per the backend code in `Userflows (1).py`.

### 4. Run the Backend Server
```
python "Userflows (1).py"
```
- The Flask server will start at `http://127.0.0.1:5000/` by default.

### 5. Run the Frontend
- Open `Frontend.html` in your web browser.
- The frontend communicates with the backend API for registration, sign-in, and dashboard features.

## API Endpoints (Backend)
- `POST /register` — Register a new user
- `POST /signin` — User sign-in
- `GET /profile/<customer_id>` — Get user profile
- `GET /eventplan/<eventplan_id>` — Get event plan details
- `GET /user/<customer_id>/eventplans` — Get all event plans for a user
- `GET /eventplan/<eventplan_id>/vendors` — Get vendors for an event plan
- `GET /eventplan/<eventplan_id>/tasks` — Get tasks for an event plan
- `POST /cart/add` — Add event plan to cart
- `GET /user/<customer_id>/homepage` — Get user's homepage event plans

## Contribution Guidelines
1. Fork the repository and create a new branch for your feature or bugfix.
2. Make your changes and test thoroughly.
3. Submit a pull request with a clear description of your changes.

## License
This project is for educational and demonstration purposes. Please contact the author for other uses.

## Credits
Developed by Kshitiz Trigunayat and contributors. 