# Use an official Node runtime as the parent image
FROM node:lts

RUN mkdir /app

# Set the working directory in the container to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
ADD . /app

# Make the container's port 80 available to the outside world
EXPOSE 8080

# Run app.js using node when the container launches
CMD ["python", "manage.py", "runserver", "0.0.0.0:8080"]