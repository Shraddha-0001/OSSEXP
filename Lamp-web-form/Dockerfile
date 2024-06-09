FROM php:7.4-apache
RUN docker-php-ext-install mysqli
COPY src/ /var/www/html/

# Use the official PHP image with Apache
FROM php:7.4-apache

# Install MySQLi extension
RUN docker-php-ext-install mysqli

# Copy the contents of the src directory to the root of the container's filesystem
COPY src/ /

# Optionally, expose the default port for the Apache web server
EXPOSE 80
