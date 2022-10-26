FROM node:14-alpine as react-build

WORKDIR /react

COPY package.json .

RUN npm install

COPY . .

RUN [ "npm", "run", "build" ]

FROM python:3

WORKDIR /django

COPY requirements.txt /django/