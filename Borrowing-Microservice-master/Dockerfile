# Use the Node.js base image
FROM node:20

# Set the working directory
WORKDIR /Borrowing-Microservice-master

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy application files
COPY . .

# Expose the application port
EXPOSE 3003

# Start the application
CMD ["node", "index.js"]
