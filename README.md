# FastAPI Example

A simple FastAPI application to manage a list of items.

## Endpoints

- `GET /`: Returns a simple `{"Hello": "World"}` message.
- `POST /items`: Create a new item. Expects a JSON payload with `text` (optional) and `is_done` (optional, defaults to false).
- `GET /items`: List items. Accepts an optional `limit` query parameter (defaults to 10).
- `GET /items/{item_id}`: Retrieve a specific item by its ID (index in the list).

## Setup & Getting Started

1. Create a virtual environment:
   ```bash
   python3 -m venv venv
   ```

2. Activate the virtual environment:
   ```bash
   source venv/bin/activate
   ```

3. Install the required dependencies:
   ```bash
   pip install fastapi uvicorn
   ```

4. Run the application:
   ```bash
   uvicorn main:app --reload
   ```

5. Visit `http://127.0.0.1:8000/docs` in your browser to see the automatic interactive API documentation provided by Swagger UI.
