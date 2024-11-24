# Specify Base image
# FROM docker.io/alpine - alpine does not create nodejs
FROM docker.io/node:18-alpine

# Work Directory
WORKDIR /usr/app

# Copy the package.json in to the container
COPY ./package.json ./

#Install Dependencies
RUN npm install

# Copy the rest of the files
COPY ./ ./

# StartUp command
CMD ["npm", "start"]
