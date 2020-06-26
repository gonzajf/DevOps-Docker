FROM ubuntu:16.04 

WORKDIR /exercise7
RUN apt-get update && apt-get install -y curl  
COPY exercise7.sh .
RUN ["chmod", "+x", "exercise7.sh"]
CMD ["/bin/bash", "exercise7.sh"]