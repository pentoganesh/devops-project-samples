FROM node:8-onbuild

# FROM node:6.9.3
LABEL maintainer="Azure App Service Container Images <appsvc-images@microsoft.com>"

# Create app directory
WORKDIR /app

# Install app dependencies
COPY package.json .

RUN npm install

# Bundle app source
COPY . .

EXPOSE 8080 8080
CMD [ "npm", "start" ]
