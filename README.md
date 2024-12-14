# recipe-app-api
UDEMY Create an advanced REST API with Python, Django REST Framework and Docker using Test Driven Development (TDD)

# Run linting tool

docker compose  run --rm app sh -c "flake8"

# Create Django Project

docker compose run --rm app sh -c "django-admin startproject app ."

# Run Test
docker compose run --rm app sh -c "python manage.py test"

# Create new App Named Core
docker compose run --rm app sh -c "python manage.py startapp core"

# Run django custom command
docker compose run --rm app sh -c "python manage.py wait_for_db"

# disable flake8 liniting
add # noqa to admin.py and models.py

# create migrations
docker compose run --rm app sh -c "python manage.py makemigrations"

# run migrations
docker compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"