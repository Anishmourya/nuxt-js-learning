FROM node:12.9-alpine

MAINTAINER Anish kumar Dhanka <anish.mourya5@gmail.com>

RUN mkdir -p  /app

WORKDIR /app

COPY package.json /app

COPY ./ /app

RUN yarn install

RUN yarn run build

# expose port
EXPOSE 3000

# Running the app
CMD [ "yarn","run","start" ]


