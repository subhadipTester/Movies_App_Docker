FROM node:14

WORKDIR /client

ENV PATH /client/node_modules/.bin:$PATH

COPY package*.json ./

COPY yarn.lock ./

RUN yarn

COPY . ./

EXPOSE 8000

CMD ["yarn", "start"]
