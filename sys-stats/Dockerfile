FROM node:10.15.2-alpine

LABEL maintainer="René Mifsud"
LABEL description="Red Acre Devops Test"

RUN mkdir /frontend

WORKDIR /frontend

COPY . /frontend
COPY package.json /frontend/package.json


RUN npm install

ENTRYPOINT [ "npm", "start" ]