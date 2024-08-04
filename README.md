# Practice - New Project with CI/CD

This guide helps you set up a micro-application using Python Flask with CI/CD, including a linter, unit tests, integration tests, and security tests.

## Tools Used
- *Bandit*: Scans Python code for security vulnerabilities.
- *Safety*: Ensures code security.

## Steps

### Step 1: Setup Flask Project
1. Create a virtual environment.
2. Structure your project:
    plaintext
    flask_app/
    ├── app/
    │   ├── __init__.py
    │   └── routes.py
    ├── tests/
    │   ├── __init__.py
    │   ├── test_routes.py
    │   ├── test_integration.py
    ├── .github/
    │   └── workflows/
    │       └── ci.yml
    ├── venv/
    ├── .flaskenv
    ├── .gitignore
    ├── .flake8
    ├── requirements.txt
    └── run.py
    

### Step 2: Configure Linter
1. Install and configure Flake8.

### Step 3: Write Unit Tests
1. Configure pytest.
2. Write tests in tests/test_routes.py.

### Step 4: Setup GitHub Actions
1. Create ci.yml in .github/workflows/.

### Step 5: Add Integration Tests
1. Write tests in tests/test_integration.py.

### Step 6: Add Security Tests
1. Use Bandit and Safety.
2. Update GitHub Actions workflow.

### Step 7: Update Dependencies
1. Maintain requirements.txt.

### Step 8: Upload to GitHub
1. Verify workflows.
2. Report on CI/CD pipeline benefits and security improvements.

## Conclusion

Follow these steps to set up a secure and automated development workflow using Python Flask and CI/CD practices.

