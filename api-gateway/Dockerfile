# FROM node:latest
# WORKDIR /app
# COPY . /app
# RUN npm install
# EXPOSE 8000
# CMD ["npm","start"]
# Use an official Node.js runtime as a parent image
FROM node:latest

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the local code to the container
COPY . .

# Expose the port the app runs on
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]
