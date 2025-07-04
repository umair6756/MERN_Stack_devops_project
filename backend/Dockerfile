# Use Node.js LTS base image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy rest of the app
COPY . .

# Expose port (change if your backend uses a different one)
EXPOSE 5000

# Start the app
CMD ["npm", "start"]
