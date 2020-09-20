FROM node:14.11.0-alpine

RUN apk add --no-cache yarn && yarn install

WORKDIR /app

CMD yarn encore dev --watch
