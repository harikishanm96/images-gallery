# Use a Python base image
FROM python:3.9-slim

# Set the working directory
WORKDIR /app

# Copy the requirements.txt into the container
COPY requirements.txt /app/

# Install dependencies including a specific version of itsdangerous
RUN pip install --no-cache-dir -r requirements.txt && pip install "itsdangerous==2.0.1"

# Copy the rest of the application files
COPY . /app

# Expose the port the app runs on
EXPOSE 5050

# Run the application
CMD ["python", "main.py"]