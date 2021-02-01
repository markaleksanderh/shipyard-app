Note taking app

Following:
https://testdriven.io/blog/dockerizing-flask-with-postgres-gunicorn-and-nginx/#project-setup

Run `docker-compose build` then `docker-compose up` to build app.

To seed database:

`docker-compose exec web python manage.py seed_db`

Shell into db:

`docker-compose exec db psql --username=username --dbname=dbname`

To run production:

`docker-compose -f docker-compose.prod.yml up -d --build`