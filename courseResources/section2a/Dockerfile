# Use the official Node.js image as the base image
FROM node

# Set the working directory inside the container
WORKDIR /app

# Copy package.json to the working directory inside the container
COPY package.json /app

# Install the dependencies specified in package.json
RUN npm install

# Copy the current directory contents into the container at /app
COPY . /app

# Expose port 80 to allow external access to the server
EXPOSE 80

# Run the server when the container starts
CMD ["node", "server.js"]