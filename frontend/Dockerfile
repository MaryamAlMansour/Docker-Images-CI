# choosing the base image
FROM node:10-alpine

# Create app directory
WORKDIR /app

# ensure both package.json AND package-lock.json are copied to the image
COPY package*.json ./

# install app depandencies
RUN npm install

# bundle the app source
COPY . .

#exposing the web port for container
EXPOSE 3000

# starting the app
CMD ["node", "index.js"]
