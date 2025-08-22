#H1 📦 GeoMap Django Web Application

A modern full-stack Django web application with an interactive Leaflet.js mapping system, designed for geolocation, marker placement, and customizable map layers. Built with Django, JavaScript, and Leaflet, it supports optional database backends and strong security practices.

🧰 Features

Django web framework (backend)

Leaflet.js interactive mapping system (frontend)

SQLite or PostgreSQL (optionally MongoDB)

Add, edit, and display map markers dynamically

Customizable map tiles & layers

Optional Docker containerization

Hardened with OWASP security practices

🧑‍💻 Getting Started (Run from Source)
📋 Prerequisites

Python 3.8+

Git

pip

🔧 Installation Steps
# Clone the repository
git clone https://github.com/yourusername/geomap-django-app.git
cd geomap-django-app

# Set up virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt

# Run initial migrations
python manage.py migrate

# Create superuser (optional)
python manage.py createsuperuser

# Run the server
python manage.py runserver

🌍 Access App

Open your browser and go to:
👉 http://127.0.0.1:8000/

Navigate to the map view to interact with the Leaflet-based GeoMap system.

🐳 Running via Docker (Recommended)
📋 Prerequisites

Docker

Docker Compose

🚀 Build & Run
# Build the Docker image
docker-compose build

# Start the container
docker-compose up


The app will be available at:
👉 http://localhost:8000/

🛠 Optional: .env file for secrets

Create a .env file if you need to inject environment variables (e.g., SECRET_KEY, DEBUG, DATABASE_URL, etc.)

Example .env:

SECRET_KEY=your-secret-key
DEBUG=True
DATABASE_URL=sqlite:///db.sqlite3

🔑 Default Admin Access (For Demo)

If you’re hosting a public version, create an admin user:

python manage.py createsuperuser


Follow the prompts to set a username, email, and password.
