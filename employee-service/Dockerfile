FROM node:18.17.0-alpine

# Set the Current Working Directory inside the container
WORKDIR /usr/src/app

# Copy dependencies package list
COPY package*.json ./
# Install dependencies
RUN npm i -g npm \
    && npm i

# Copy all source code
COPY . .

# Expose application port
EXPOSE 8004

# Run application
CMD ["npm","start"]
