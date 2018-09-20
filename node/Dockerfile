FROM node:8.12.0-jessie
RUN apt-get update && apt-get install vim -y
RUN mkdir /var/node-app
WORKDIR /var/node-app
RUN npm init -y
RUN npm install express body-parser morgan mongoose jsonwebtoken --save
ADD node-app /var/node-app

EXPOSE 8080

CMD ["/usr/local/bin/node", "server.js"]
