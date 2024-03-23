Event Finder RESTful API
Introduction
This is a RESTful service that manages and queries event data based on a user's geographical location and a specified date. The service ingests data from a provided CSV dataset and offers an API to find events for users.

Features
Data Creation API: Add events into the system using details provided in the CSV dataset (event name, city name, date, time, latitude, longitude).
Event Finder API: List events based on the user's latitude, longitude, and a specified date. The system returns events occurring within the next 14 days from the specified date, sorted by the earliest event after the specified date.
Core Requirements
Data Creation API Endpoint: /events/create
Event Finder API Endpoint: /events/find
External APIs
Weather API: Retrieve weather conditions for an event based on its location and date.
Endpoint: https://gg-backend-assignment.azurewebsites.net/api/Weather
Distance Calculation API: Calculate the distance between the user's location and the event location.
Endpoint: https://gg-backend-assignment.azurewebsites.net/api/Distance
Tech Stack
Backend Framework: Flask (Python)
Database: CSV file
External APIs: Weather API, Distance Calculation API
Setup
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/event-finder-api.git
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Run the Flask application:

bash
Copy code
python app.py
The API server will start running at http://localhost:5000.

API Documentation
Detailed documentation for API endpoints, request/response formats, and error codes can be found here.

Justification and Reflection
For a brief report explaining the choice of tech stack, database, design decisions, and how challenges were addressed, refer to this document.

