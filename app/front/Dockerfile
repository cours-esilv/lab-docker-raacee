# Use the official Nginx base image
FROM nginx:latest

# Copy the local files into the container at /usr/share/nginx/html/
COPY . /usr/share/nginx/html/

# Copy the entrypoint script into the container
COPY entrypoint.sh /usr/share/nginx/

# Set the execute permission for the entrypoint script
RUN chmod +x /usr/share/nginx/entrypoint.sh

# Specify the entrypoint script to be run when the container starts
ENTRYPOINT ["/usr/share/nginx/entrypoint.sh"]

# Expose port 80 to the outside world
EXPOSE 8080
