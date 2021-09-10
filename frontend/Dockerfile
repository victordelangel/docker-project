FROM node:current-alpine3.11

WORKDIR /usr/app

COPY package.json .
COPY yarn.lock .

RUN yarn install

COPY . .

EXPOSE 3000

ENTRYPOINT ["yarn","start"]