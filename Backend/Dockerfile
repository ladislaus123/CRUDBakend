# Use official Node.js image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install --production

# Copy the rest of the code
COPY . .

# Expose port (the one your Express app listens on)
EXPOSE 3000

# Start the app
CMD ["node", "index.js"]
