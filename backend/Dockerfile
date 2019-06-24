FROM node:10.16.0-alpine

WORKDIR /usr/app

VOLUME [ "/usr/app" ]

RUN npm install -g nodemon
RUN npm run test

ENV NODE_ENV=development
ENV DATABASE=mongodb://mongodb:27017/mean
ENV PORT=3000

EXPOSE 3000

CMD [ "nodemon", "-L", "src/index.js" ]
