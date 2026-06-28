# FastAPI Example

A simple FastAPI application to manage a list of items.

## Endpoints

- `GET /`: Returns a simple `{"Hello": "World"}` message.
- `POST /items`: Create a new item. Expects a JSON payload with `text` (optional) and `is_done` (optional, defaults to false).
- `GET /items`: List items. Accepts an optional `limit` query parameter (defaults to 10).
- `GET /items/{item_id}`: Retrieve a specific item by its ID (index in the list).

## Getting Started

1. Activate your virtual environment (if you are using the provided `venv`):
   ```bash
   source venv/bin/activate
   ```

2. Run the application (assuming you have `uvicorn` installed):
   ```bash
   uvicorn main:app --reload
   ```

3. Visit `http://127.0.0.1:8000/docs` in your browser to see the automatic interactive API documentation provided by Swagger UI.
