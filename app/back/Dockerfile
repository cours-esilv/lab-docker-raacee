# Use an official Python runtime as a parent image
FROM python:3.9

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Make port 5000 available to the world outside this container
EXPOSE 5000

# Set the environment variable
ENV CURRENT_ENVIRONMENT production

# Run the specified command within the container
CMD ["python", "-m", "flask", "run", "--host=0.0.0.0"]

