# Use official Node.js image
FROM node:18

# Create a folder inside container
WORKDIR /app

# Install only dependencies first
COPY package.json package-lock.json* ./
RUN npm install --production

# Copy the rest of the project
COPY . .

# Expose backend port
EXPOSE 5000

# Start server
CMD ["npm", "start"]
