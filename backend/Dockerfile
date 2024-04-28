FROM node:21-alpine

WORKDIR	/app

COPY . .

RUN npm i

RUN npm run test

COPY .env.docker .env

EXPOSE 5000

CMD ["npm","start"]
