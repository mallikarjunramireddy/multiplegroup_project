# Use an official Python runtime as a parent image
FROM python:3.12.3-alpine3.19

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed dependencies specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Set Database environment variable
ENV MONGO_URI mongodb://mongodb:27017/

# Expose port 5000 to allow communication to/from server
EXPOSE 5000

# Command to run the application
CMD ["python", "app.py"]
