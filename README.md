# FastAPI Token Verifier

This project is a FastAPI service that verifies tokens received from a frontend application. It provides an API endpoint to validate tokens and return user information or an authentication failure response.

## Project Structure

```
.
├── main.py
├── pyproject.toml
├── README.md
├── requirements.txt
└── uv.lock
```

## Setup Instructions

1. Clone the repository:
   ```
   git clone <repository-url>
   cd cheveningbrew-auth-server
   ```

2. Create a virtual environment:
   ```
   python -m venv .venv
   source .venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

To run the FastAPI application, execute the following command:

```
python -m uvicorn main:app --reload --port 8001
```

The application will be available at `http://127.0.0.1:8001`.

## API Endpoints

- **POST "/api/auth/google"**
  - Description: Verifies the provided token.
  - Request Body: Token data in JSON format.
  - Response: User information or authentication failure message.

## License

This project is licensed under the MIT License.# cheveningbrew-user-auth-server
