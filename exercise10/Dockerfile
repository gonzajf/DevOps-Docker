FROM ubuntu:16.04 

WORKDIR /exercise10
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs
COPY frontend-example-docker-master /exercise10
RUN npm install
EXPOSE 5000
CMD ["npm", "start"]