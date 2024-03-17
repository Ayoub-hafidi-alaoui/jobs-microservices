# base image
FROM python:3.11-slim-bullseye

ENV PYTHONUNBUFFERED=1

# update
RUN apt-get update && apt-get -y install gcc libpq-dev

# create default folder
WORDIR /app

COPY requirements.txt /app/requirements.txt

RUN pip install -r requirements.txt


# COPY all projects files
COPY . /app/
