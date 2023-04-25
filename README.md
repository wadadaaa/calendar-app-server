# Calendar App Server

This is the server-side application for the Calendar App. It is built using Python and uses the FastAPI framework to provide a RESTful API for the app.

## Prerequisites

Before running the server, make sure you have the following installed:

- Python 3.8+
- pip

## Installation

1. Clone the repository: `git clone https://github.com/YOUR_USERNAME/calendar-app-server.git`
2. `cd calendar-app-server`
3. Install the dependencies: `pip install -r requirements.txt`

## Running the Server

To run the server, execute the following command in your terminal:

```bash
uvicorn main:app --reload
```

This will start the server on `http://localhost:8000`.

## API Endpoints

The following endpoints are available:

### GET /events

Returns a list of all events.

### GET /events/{event_id}

Returns a specific event.

### POST /events

Creates a new event.

### PUT /events/{event_id}

Updates an existing event.

### DELETE /events/{event_id}

Deletes an event.

## Usage with Calendar App Frontend

To use the server with the Calendar App frontend:

1. Follow the instructions in the Calendar App frontend repository to install and run the app.
2. Update the `API_URL` constant in `src/components/CalendarView.js` to point to your local server instance: `http://localhost:8000` (assuming you're running the server locally).
3. Start the server by running the command mentioned in the previous section.

You should now be able to use the Calendar App with your local server instance.
