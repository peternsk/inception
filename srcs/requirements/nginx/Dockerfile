FROM    debian:bullseye-slim

RUN     apt update -y && apt upgrade -y \
        && apt install -y nginx &&  \
        apt install openssl -y

RUN     openssl req -x509 -nodes -days 365 \
        -newkey rsa:2048 -keyout /etc/ssl/private/nginx-selfsigned.key \ 
        -out /etc/ssl/certs/nginx-selfsigned.crt \ 
        -subj "/C=MO/L=KH/O=1337/OU=student/CN=[pnsaka.1337.fr](http://pnsaka.42.fr/)"