# Use Node base image
FROM node:14-alpine

# Set working directory inside container
WORKDIR /usr/src/app

# Copy package.json first
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy rest of the code
COPY . .

# Expose port
EXPOSE 3000

# Start CRA dev server
CMD ["npm", "start"]
