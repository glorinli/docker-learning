# Use an official python runtime as a parent image
FROM python:2.7-slim

# Set the working directory
WORKDIR /app

# Copy the current directory contents
COPY . /app

# Install packages
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# make 80 port avaiable to the world outside this container
EXPOSE 80

# Define environment variable
ENV NAME World

# Run app.py when the container launches
CMD ["python", "app.py"]
