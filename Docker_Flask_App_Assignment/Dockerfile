# Using the official Python 3.9-slim image
FROM python:3.9-slim

# Setting the working directory inside the container
WORKDIR /flask-app

# Copying the Flask application code and requirements.txt file to the container
COPY . /flask-app/
COPY requirements.txt /app/

# Installing Flask directly using pip
RUN pip install --no-cache-dir -r requirements.txt

# Exposing port 5000 to allow incoming HTTP traffic to the container
EXPOSE 5000

# Specifying the command to run the Flask application when the container starts
CMD ["python", "app.py"]



