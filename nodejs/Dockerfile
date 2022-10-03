FROM node:9-alpine
LABEL MAINTAINER="iamkoldzo@gmail.com"

RUN apk update
RUN apk add git
RUN git clone https://github.com/kkenan/basic-microservices.git
RUN mv basic-microservices/node-app /node-app
RUN rm -r basic-microservices/

WORKDIR /node-app

RUN npm install

ENTRYPOINT ["node", "index.js"]
