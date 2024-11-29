FROM node:20

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install

COPY . .
COPY .env ./

ENV Node_ENV=production
EXPOSE 8080
CMD ["npm", "run", "start"]