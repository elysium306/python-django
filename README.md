# python-django

# Run All commands through Docker Compose

> docker-compose run --rm app sh -c "python manage.py collectstatic"

# To run a Docker Compose command

> docker-compose

# To start a specific container defined in config

> run

# To remove the container

> --rm

# Name of the service

> app

# To pass a shell command

> sh -c

# The command to run inside container

>

# Below is the command we need to run before everyone command we need to run

> docker-compose run --rm app

# Starting from <sh -c> is actually the command we need to run on the container

> sh -c "python manage.py collectstatic

---

    - Install 'flake8'
    - Run it through Docker Compose
        > docker-compose run --rm app sh c- "flake8"
    - If there is any linting issue, work the way up -- start from the last error, and fix one by one
        - the reason being, if we work from the top-down direction, it's gonna chnage the line number as we need more lines of codes, then it may be difficult to fix the rest of the errors.

# Testing:

    - for testing, we will be using Django test suite
    - Setup tests per Django app
    - Run tests through Docker Compose

        > docker-compose run --rm app sh -c "python manage.py test"

# To create the Django project inside the Docker Compose, run:

    > docker-compose run --rm app sh -c "django-admin startproject app ."
