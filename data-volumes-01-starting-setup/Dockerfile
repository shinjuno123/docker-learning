FROM node:14

WORKDIR /node-app

COPY package.json .

RUN npm install

COPY . .

ARG DEFAULT_PORT=80

ENV PORT $DEFAULT_PORT

EXPOSE $PORT

# VOLUME [ "node","server.js" ]

CMD ["npm","start"]