FROM ubuntu:16.04


RUN apt-get update 
RUN apt-get install -y apache2 
RUN apt-get install -y apache2-utils 
RUN apt-get clean

COPY index.html /var/www/html/

# Run the server on port 80
EXPOSE 80

# Run te server after set up
CMD ["apache2ctl", "-D", "FOREGROUND"]
