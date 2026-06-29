# Use Node.js base image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files first
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install --legacy-peer-deps

# Copy backend source code
COPY . .

# Expose backend port
EXPOSE 3001

# Start the server
CMD ["node", "index.js"]
