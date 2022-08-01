#  pull the official base image
FROM python:3.10.4-slim-buster

# Set the working directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Set env variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Install dependencies
RUN python -m pip install --upgrade pip
COPY ./requirements.txt .
RUN python -m pip install -r requirements.txt

# Add app
COPY . .
