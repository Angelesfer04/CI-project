# Flask App with CI/CD

This project is a simple Flask application with a CI/CD pipeline. It includes linting, unit tests, integration tests, and security tests.

## Project Structure

flask_app/
├── app/
│ ├── init.py
│ └── routes.py
├── tests/
│ ├── init.py
│ ├── test_routes.py
│ ├── test_integration.py
├── .github/
│ └── workflows/
│ └── ci.yml
├── venv/
├── .flaskenv
├── .gitignore
├── .flake8
├── requirements.txt
└── run.py

bash
Copy code

## Setup

1. Create the Virtual Environment:
   ```bash
   python -m venv venv
   source venv/bin/activate
Install Dependencies:
bash
Copy code
pip install -r requirements.txt
Running the Application
bash
Copy code
python run.py
Running Tests
bash
Copy code
flake8 .
pytest
bandit -r app
safety check
CI/CD Workflow
The project uses GitHub Actions for CI/CD. The workflow is defined in .github/workflows/ci.yml and includes the following steps:

Checkout code
Set up Python
Install dependencies
Lint with Flake8
Test with pytest
Security check with Bandit
Dependency check with Safety
Security Tools
Bandit: A tool to find common security issues in Python code.
Safety: Checks installed dependencies for known security vulnerabilities.
