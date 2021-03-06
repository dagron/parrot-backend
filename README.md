# parrot-backend
> The backend service of "PARROT".

## Environments
- Language: Python 3.7
- Framework: Flask 1.1
- WSGI Server: Gunicorn
- Deploy: Cloud Run

## Project setup
```
# install requirements
$ pip install pipenv
$ pipenv run init

# activate
$ pipenv shell
```

- Container
```
# build docker image
$ docker build -t $(DOCKER_TAG_NAME) .
```

## Run application
```
# compiles and hot-reloads
$ pipenv run start
```

- Container
```
# run docker container
$ docker container run --rm -p 5000:5000 $(DOCKER_TAG_NAME)
```

## Extras
```
# type check
$ pipenv run type

# lint
$ pipenv run lint

# format
$ pipenv run format
```