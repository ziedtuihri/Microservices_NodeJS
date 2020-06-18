FROM node:10.16.0-alpine

WORKDIR /app

ADD ./package.json /app/

RUN npm install express -g

RUN npm install mongodb -g

COPY package*.json ./

RUN npm install

ADD ./ /app/src/

CMD ["node", "src/index.js"]