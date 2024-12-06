FROM node:20

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install

COPY . .

COPY ./certs/global-bundle.pem /etc/ssl/certs/global-bundle.pem


ENV NODE_ENV=production
EXPOSE 8080
CMD ["npm", "run", "start"]