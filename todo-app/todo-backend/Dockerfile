FROM node:16

WORKDIR /usr/src/app

COPY . .

RUN npm ci

CMD PORT=12600 npm run dev