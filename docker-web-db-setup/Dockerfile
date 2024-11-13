# Use official Ubuntu base image
FROM ubuntu:20.04

# Install Nginx and MySQL server
RUN apt-get update && \
    apt-get install -y nginx mysql-server mysql-client && \
    apt-get clean

# Expose web and MySQL ports
EXPOSE 80 3306

# Start both Nginx and MySQL services
CMD service mysql start && nginx -g 'daemon off;'
