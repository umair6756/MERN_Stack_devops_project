# Base image with Node and Yarn
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package.json yarn.lock ./
RUN yarn install

# Copy the rest of the app
COPY . .

# Expose the React development server port
EXPOSE 3000

# Start the app in development mode
CMD ["yarn", "start"]
