FROM node:26.3.0-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install 
RUN npm install && npm update serve-static send qs path-to-regexp mpath mongoose
COPY . . 
EXPOSE 8080
CMD ["node" , "index.js"] 
