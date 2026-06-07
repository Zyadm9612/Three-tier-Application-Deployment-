FROM node:26.3.0-alpine 
WORKDIR /app 
COPY package*.json ./ 
RUN npm install 
RUN npm install && npm update ws webpack-dev-middleware url-parse terser sha.js 
COPY . . 
EXPOSE 3000
CMD [ "npm" , "start" ] 
