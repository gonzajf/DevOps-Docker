FROM ubuntu:16.04

WORKDIR /usr/src/app

RUN apt-get update && apt-get install -y curl && \
	curl -sL https://deb.nodesource.com/setup_10.x | bash && \
	apt install -y nodejs	&& \
	apt-get purge -y --auto-remove curl && \
	rm -rf /var/lib/apt/lists/*

COPY backend-example-docker-master /usr/src/app

RUN npm install

EXPOSE 8000

ENV FRONT_URL="http://localhost:5000"

CMD ["npm","start"]