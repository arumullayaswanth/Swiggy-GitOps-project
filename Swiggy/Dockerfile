
# Use Node.js based on Debian Slim as the base image
FROM node:16-slim

# Create and set the working directory inside the container
WORKDIR /app

# Copy the entire codebase to the working directory
COPY . .

# Install dependencies
RUN npm install

# Expose the port your app runs on
EXPOSE 3000

# Define the command to start your application
CMD ["npm", "start"]

