# Base Image 
FROM ubuntu:16.04

# MAINTAINER
MAINTAINER Amit Vashist <amitvashist7@outlook.com>

# Update APT Repo 
RUN apt-get update 

# Install Apache Packages 
RUN apt-get install apache2 -y 

# Deploy Custom Page
COPY amit.html /var/www/html/index.html

# My Service Port No. 
EXPOSE 80


# Excute the Apache Process
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
