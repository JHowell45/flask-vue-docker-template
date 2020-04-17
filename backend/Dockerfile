FROM python:3.7-alpine

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Updates and installations:
RUN pip install pipenv

# Setup working directory:
WORKDIR /app

## Install requirements:
COPY Pipfile Pipfile.lock ./
RUN pipenv install --deploy
