# syntax=docker/dockerfile:1
FROM node:alpine
ENV NODE_ENV=dev
WORKDIR /app
COPY ["package.json", "package-lock.json*", "./"]
RUN npm install --omit=dev
COPY . .
EXPOSE 8080
CMD [ "node", "server.js" ]