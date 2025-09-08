# Use Node base image
FROM node:14-alpine

# Set working directory inside container
WORKDIR /usr/src/app

# Copy package.json first (to leverage Docker caching)
COPY package.json ./

# Install dependencies
RUN npm install

# Copy rest of the code
COPY . .

# Expose backend port
EXPOSE 5000

# Start the app
CMD ["npm", "start"]
