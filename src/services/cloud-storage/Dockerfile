FROM node:8

# Create app directory
WORKDIR /usr/src/app

COPY package.json ./

COPY yarn.lock ./

RUN yarn

# Bundle app source
COPY scripts scripts/
COPY *.js ./

EXPOSE 8080

CMD [ "npm", "start" ]