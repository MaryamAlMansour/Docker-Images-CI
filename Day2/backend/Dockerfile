FROM node:10-alpine

# Create app directory
WORKDIR /app

# ensure both package.json AND package-lock.json are copied to the image
COPY package*.json ./

# install app depandencies
RUN npm install

#creating the enviromental variable to connect to postgres
#ENV API_URL="postgres://YourUserName:dojo-belt2@localhost:5432/YourDatabaseName"

#ENV API_URL="http://localhost:3000"

# bundle the app source
COPY . .

CMD ["node", "index.js"]

