FROM node:12

# create app directory
WORKDIR /usr/app

# install app dependencies
COPY package*.json ./

# install packages
RUN npm ci -qy

# bundle app source
COPY . .

EXPOSE 3000
CMD ["npm", "start"]
