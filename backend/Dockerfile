
# Use official Node.js lightweight image
FROM node:22-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install production dependencies
RUN npm install --omit=dev

# Copy backend source code
COPY src/ ./src/

# Application port
EXPOSE 3000

# Run as non-root user
USER node

# Start backend application
CMD ["npm", "start"]
