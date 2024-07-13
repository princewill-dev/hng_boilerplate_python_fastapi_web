# FASTAPI

FastAPI boilerplate

 

## Setup

 

1. Create a virtual environment.

 ```sh

    python3 -m venv .venv

 ```

2. Activate virtual environment.

```sh

    source /path/to/venv/bin/activate`

```

3. Install project dependencies `pip install -r requirements.txt`

4.

5. Create a .env file by copying the .env.sample file

`cp .env.sample .env`

 

1. Start server.

 ```sh

 python main.py

```

2. The API will be available at http://127.0.0.1:8000.

3. Running Tests

 To ensure the functionality and stability of the application, we use pytest for running both unit tests and end-to-end tests. Our tests cover various aspects of the application, including:

 

Database Operations: Verifying that CRUD operations work correctly with the database.

API Endpoints: Ensuring that the API endpoints behave as expected.

Dependency Injection: Overriding dependencies for testing purposes to ensure isolation and repeatability of tests.

Setting Up the Test Environment

We use a separate test database to run our tests. The database schema is recreated before each test to ensure a clean state. This is handled by the session fixture.

 

The client fixture creates a test client that overrides the database dependency with the test database session, allowing us to send HTTP requests to the API endpoints during testing.

 

''sh

  pytest

''''

4. API Documentation

The API documentation is generated automatically by FastAPI and can be accessed at:

 

Swagger UI: http://127.0.0.1:8000/docs

ReDoc: http://127.0.0.1:8000/redoc

 

5. License

This project is licensed under the MIT License - see the LICENSE file for details.




