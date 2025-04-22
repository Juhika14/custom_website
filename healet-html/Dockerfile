FROM ubuntu:20.04

# Install Apache
RUN apt update && apt install -y apache2 && apt clean

# Copy website files into Apache's root directory
COPY . /var/www/html/

# Expose port 80
EXPOSE 80

# Start Apache in foreground
CMD ["apachectl", "-D", "FOREGROUND"]
