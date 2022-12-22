# Dockerize a simple Python script with third-party modules

We differ between:

- Dockerfile: Blueprint for building images
- Image: Template for running containers
- Container: Running process with the packaged project

## How to Get Started

## 1. Build the Docker image

```console
$ docker build -t python-imdb .
```

## 2. Run the Docker image (starts the container)

Without user input:

```console
$ docker run python-imdb
```

With user input

- Comment out the 'break' in [main.py](./main.py):

```console
$ docker run -it python-imdb
```

-i: intreactive, -t: pseudo terminal

*rebuild image [#1] when code is changed
