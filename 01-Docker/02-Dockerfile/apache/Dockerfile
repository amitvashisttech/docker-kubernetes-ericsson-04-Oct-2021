# Base Image 
FROM ubuntu:16.04 

# Update the APT Repo 
RUN apt-get update 

# Install Apache Packages 
RUN apt-get install apache2 -y 

# Copy Custom Web Page.
COPY index.html /var/www/html/

# My App Expose on Port 80.
EXPOSE 80 

# Bring the Apache Up. 
CMD ["/usr/sbin/apache2ctl", "-D" , "FOREGROUND"]
