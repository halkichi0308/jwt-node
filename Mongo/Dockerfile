FROM debian:latest
RUN apt-get update && apt-get install mongodb -y
RUN mkdir /data && mkdir /data/db
EXPOSE 27017

ENTRYPOINT ["/usr/bin/mongod"]
