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
