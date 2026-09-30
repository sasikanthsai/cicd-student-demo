# Student CI/CD Demonstration

This project demonstrates Continuous Integration and Continuous Deployment using GitHub Actions.

## Pipeline

Code Push
    |
    v
Continuous Integration
    |
    +-- Set up Python
    +-- Install pytest
    +-- Run automated tests
    |
    v
Tests PASS?
    |
    +-- NO  -> Stop
    |
    +-- YES
          |
          v
Continuous Deployment
          |
          +-- Configure GitHub Pages
          +-- Upload website
          +-- Deploy website
          |
          v
      Live Website

## Files

- `student_result.py` - Python application
- `test_student_result.py` - automated tests
- `index.html` - webpage deployed to GitHub Pages
- `.github/workflows/ci-cd.yml` - combined CI/CD pipeline

## Expected tests

3 tests should pass:

- `test_pass`
- `test_fail`
- `test_boundary`

## GitHub Pages

In the repository:

Settings -> Pages -> Build and deployment -> Source -> GitHub Actions

After a successful deployment, GitHub will provide the Pages URL.
