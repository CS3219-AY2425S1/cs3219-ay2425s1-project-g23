# Dockerfile for user-service
FROM node:20-alpine

ARG PORT

WORKDIR /app

COPY package*.json ./

RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the service port
EXPOSE $PORT

# Start the user service
CMD ["npm", "start"]