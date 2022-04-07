FROM node:17-alpine
# Parent layer node with alpine(lightweight linux distribution)

RUN npm install -g nodemon
# Installing nodemon to listen for changes in the code and restart the server

WORKDIR /app
# Creating a dir in container

COPY package.json .
# . means current dir
# Copying package.json that contains metadata about our dependencies to container 

RUN npm install
# RUN npm install to install those dependencies

COPY . .
# Copy the rest of dir to container

EXPOSE 4000
# Required for docker desktop port mapping

CMD ["npm", "run", "dev"]
# Using a script to run the app using nodemon