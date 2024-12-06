# base image
FROM node:20-alpine

# working directory
WORKDIR /app

# copy the package.json and package-lock.json files
COPY package*.json ./

# install the dependencies
RUN npm install

# copy the rest of the application files
COPY . .

# Expose the port our app will run on
EXPOSE 3000

# start our application
CMD ["npm", "start"]