# TDD and CI/CD Demo Project

[![codecov](https://codecov.io/gh/rayluo88/cicd-demo/branch/main/graph/badge.svg)](https://codecov.io/gh/rayluo88/cicd-demo)

This project demonstrates Test-Driven Development (TDD) and Continuous Integration/Continuous Deployment (CI/CD) concepts using a simple calculator library.

## Concepts Demonstrated

### Test-Driven Development (TDD)
- Writing tests before implementation
- Red-Green-Refactor cycle
- Unit testing best practices

### CI/CD
- Automated testing
- Continuous Integration with GitHub Actions
- Automated deployment workflow

## Project Structure
```
.
├── calculator/
│   ├── __init__.py
│   └── calculator.py
├── tests/
│   ├── __init__.py
│   └── test_calculator.py
├── requirements.txt
├── .github/
│   └── workflows/
│       └── ci.yml
└── README.md
```

## Setup
1. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Running Tests
```bash
pytest
```

## CI/CD Pipeline
The project uses GitHub Actions for CI/CD, which:
1. Runs on every push and pull request
2. Executes all tests
3. Checks code formatting
4. Reports test coverage 