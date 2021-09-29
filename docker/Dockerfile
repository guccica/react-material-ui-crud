# Contenerize Read-Material-UI-CRUD


# use latest LTS (long term support) version 14 of Node from Docket Hub
From node:14

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY ../package*.json ./

RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY ../ .

# Expose port 3000 for the container
EXPOSE 3000

# Start the web server
CMD [ "node", "server.js" ]
