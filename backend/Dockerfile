# Use the official Node.js image
FROM node:18-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the app's code
COPY . .

# Copy .env file
# COPY .env ./

# Expose port 3000 (Nest.js default)
EXPOSE 3000

# Run the Nest.js app
CMD ["npm", "run", "start:dev"]
