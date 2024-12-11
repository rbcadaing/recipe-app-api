# recipe-app-api
UDEMY Create an advanced REST API with Python, Django REST Framework and Docker using Test Driven Development (TDD)

# Run linting tool

docker compose  run --rm app sh -c "flake8"

# Create Django Project

docker compose run --rm app sh -c "django-admin startproject app ."

# Run Test
docker compose run --rm app sh -c "python manage.py test"