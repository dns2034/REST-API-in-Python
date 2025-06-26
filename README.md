# Travel API

## Overview

The Travel API is built using Flask and SQLAlchemy. It allows users to manage travel destinations, including creating, reading, updating, and deleting destination entries in a SQLite database.

## Features

- **Home Route**: Displays a welcome message.
- **Get All Destinations**: Retrieve a list of all travel destinations.
- **Get Destination by ID**: Retrieve a specific destination by its ID.
- **Add Destination**: Add a new travel destination.
- **Update Destination**: Update an existing destination by its ID.
- **Delete Destination**: Remove a destination by its ID.

## Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
2. **Navigate to the project directory**:
   ```bash
   cd <project-directory>
3. **Install the required packages**:
   ```bash
   pip install Flask Flask-SQLAlchemy
4. **Run the application**:
   ```bash
   python app.py

## API Endpoints

### GET /

- **Description**: Welcome message.
- **URL**: `http://localhost:5000/`

---

### GET /destinations

- **Description**: Retrieve all destinations.
- **URL**: `http://localhost:5000/destinations`

---

### GET /destinations/<int:destination_id>

- **Description**: Retrieve a specific destination by ID.
- **URL**: `http://localhost:5000/destinations/2`

---

### POST /destinations

- **Description**: Add a new destination.
- **Request Body**:
  ```json
  {
    "destination": "Paris",
    "country": "France",
    "rating": 4.5
  }

---

### PUT /destinations/int:destination_id
- **Description**:  Update an existing destination.
- **Request Body**:
  ```json
  {
  "destination": "Updated Destination",
  "country": "Updated Country",
  "rating": 5.0
  }

---

### DELETE /destinations/int:destination_id
- **Description**:  Delete a destination by ID.
- **URL**: `http://localhost:5000/destinations/2`


## Postman Collection
You can test the API using Postman. Here is the link to the Postman collection:
`https://denese.postman.co/workspace/Denese's-Workspace~2c11a45e-e03b-4d2d-8b7b-2a5f350f90d1/request/45194725-65de7841-70db-4335-916c-b0d9f73123fc?action=share&creator=45194725&ctx=documentation`

## Contributing
Feel free to submit issues or pull requests for improvements or bug fixes.
