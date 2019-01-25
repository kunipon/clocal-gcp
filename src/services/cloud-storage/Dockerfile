FROM node:8

# Create app directory
WORKDIR /usr/src/app

COPY package.json ./
COPY yarn.lock ./
COPY scripts scripts/
COPY *.js ./

RUN yarn

EXPOSE 8080

CMD [ "npm", "start" ]