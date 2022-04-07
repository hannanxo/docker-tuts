FROM node:16-alpine
# Parent layer node with alpine(lightweight linux distribution)

WORKDIR /app
# Creating a dir in container

COPY package.json .
# . means current dir
# Copying package.json that contains metadata 
# about our dependencies to container 

RUN npm install
# RUN npm install to install those dependencies

COPY . .
# Copy the rest of dir to container

EXPOSE 3000
# Required for docker desktop port mapping

CMD ["npm", "start"]
# Run the application