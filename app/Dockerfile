FROM node:7.7.2-alpine

WORKDIR /app

COPY package.json .
RUN npm install -quiet
# Copy all the files from the project's root
COPY . .
EXPOSE 8080