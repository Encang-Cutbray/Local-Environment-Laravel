FROM bitnami/php-fpm:7.4-debian-10

RUN apt-get update && apt-get install -y \
    zlib1g-dev \
    libzip-dev \
    unzip 

RUN apt-get update
RUN apt-get install -y build-essential libssl-dev
RUN curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.35.1/install.sh | bash
SHELL ["/bin/bash", "--login", "-c"]
RUN nvm install node
