FROM ubuntu:16.04 

WORKDIR /exercise11
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs
COPY backend-example-docker-master /exercise11
RUN npm install
EXPOSE 8000
ENV FRONT_URL=http://localhost:5000
CMD ["npm", "start"]