# Use the official Node.js image as the base
FROM node:18-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the app's code
COPY . .

# Expose port 3000 (Next.js default)
EXPOSE 3000

# Start the Next.js development server
CMD ["npm", "run", "dev"]
