# Specify a base image
FROM node:alpine 

# Create app directory
RUN mkdir -p /usr/src/server 

# Set the working directory
WORKDIR /usr/src/server 

# Copy package.json to the working directory
COPY package.json /usr/src/server/ 

# Install app dependencies
RUN npm install 

# Copy app source code to the working directory
COPY . /usr/src/server 

# Expose the port the app runs on
EXPOSE 3000 

# The command to run the application
CMD [ "node", "server.js" ]
