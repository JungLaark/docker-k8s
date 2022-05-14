FROM ubuntu
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update
RUN apt-get install apache2 -y
ADD hello.html /var/www/html/
WORKDIR /var/www/html/
RUN ["/bin/bash", "-c", "echo hello2 >> hello2.html"]
EXPOSE 80
CMD apachectl -DFOREGROUND