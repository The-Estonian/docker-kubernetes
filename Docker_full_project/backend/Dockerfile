FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

ENV MONGODB_USER=userAdmin
ENV MONGODB_PASSWORD=superPassword

CMD ["npm", "run", "server"]
