# Ref: https://nodejs.org/fr/docs/guides/nodejs-docker-webapp/
FROM node:8

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
# A wildcard is used to ensure both package.json 
# AND package-lock.json are copied where available (npm@5+).
COPY package*.json ./
RUN npm install

# Bundle app source
COPY . .

EXPOSE 9000
EXPOSE 9001
EXPOSE 9002

# CMD ["npm", "start-client"]