FROM node:18.17.0 AS server

WORKDIR /server

COPY package*.json ./

RUN npm install --package-lock-only

COPY . .

EXPOSE 8080

CMD ["npm", "start"]