FROM python:3.7-alpine

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Updates and installations:
RUN pip install pipenv

# Setup working directory:
WORKDIR /app

## Install requirements:
RUN pipenv install --deploy
