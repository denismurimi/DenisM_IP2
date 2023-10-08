# Creating base image
FROM node:alpine3.18

# setting the working directory
RUN mkdir -p /application/client
WORKDIR /application/client

# Copying the package.json files to the working directory
COPY package*.json /application/client

# Installing the dependencies
RUN npm install --silent
# RUN npm install react-scripts@3.3.1 -g --silent

# Copying the rest of the files to the working directory
COPY . /application/client

# Running the app
CMD ["npm", "start"] 

