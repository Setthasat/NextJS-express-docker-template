FROM node:18-alpine as server
WORKDIR /app
COPY package.json ./
RUN npm install
COPY . .
COPY .env ./
EXPOSE 8888
CMD ["node", "dist/index.js"]
