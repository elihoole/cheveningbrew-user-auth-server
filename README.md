# FastAPI Token Verifier

This project is a FastAPI service that verifies tokens received from a frontend application. It provides an API endpoint to validate tokens and return user information or an authentication failure response.

## Project Structure

```
fastapi-token-verifier
├── app
│   ├── main.py                # Entry point of the FastAPI application
│   ├── api
│   │   └── v1
│   │       └── endpoints
│   │           └── token_verifier.py  # Endpoint for token verification
│   ├── core
│   │   └── config.py          # Configuration settings
│   ├── models
│   │   └── token.py           # Data model for the token
│   ├── schemas
│   │   └── token.py           # Pydantic schemas for validation
│   └── utils
│       └── token.py           # Utility functions for token handling
├── requirements.txt            # Project dependencies
└── README.md                   # Project documentation
```

## Setup Instructions

1. Clone the repository:
   ```
   git clone <repository-url>
   cd fastapi-token-verifier
   ```

2. Create a virtual environment:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

To run the FastAPI application, execute the following command:

```
uvicorn app.main:app --reload
```

The application will be available at `http://127.0.0.1:8000`.

## API Endpoints

- **POST /api/v1/verify-token**
  - Description: Verifies the provided token.
  - Request Body: Token data in JSON format.
  - Response: User information or authentication failure message.

## License

This project is licensed under the MIT License.