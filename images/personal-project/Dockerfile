FROM php:apache
RUN export DEBIAN_FRONTEND=noninteractive
RUN apt-get update
RUN apt-get install curl gcc g++ make
RUN curl -fsSL https://deb.nodesource.com/setup_16.x | bash -
RUN apt-get install apt-utils git zip vim nodejs -y
COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer