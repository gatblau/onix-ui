FROM node:alpine
MAINTAINER Gatblau <onix@gatblau.org>
WORKDIR /usr/src/app
COPY ../../package*.json ./
COPY ../../LICENSE.md ./
RUN npm install
# If you are building your code for production
# RUN npm ci --only=production
COPY . .
EXPOSE 8080
USER 20
CMD [ "npm", "start" ]