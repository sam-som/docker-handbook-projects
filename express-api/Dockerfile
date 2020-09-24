#download base node image since our app is nodejs based
FROM node
#set working directory
WORKDIR /usr/app

#copy package.json from local machine to container
COPY ./package.json ./
#run 'npm install' in the container
RUN npm install

#copy all everyting in local machine to container
COPY . .

CMD ["npm", "run", "start"]