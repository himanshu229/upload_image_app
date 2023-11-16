# Use a node base image
FROM node:16-alpine as builder

# Set the working directory
WORKDIR /client

# Copy package.json and package-lock.json files
COPY package*.json ./

# Copy the entire app directory
COPY . .

# Install dependencies
RUN npm install --package-lock-only

# Build the application
# RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]