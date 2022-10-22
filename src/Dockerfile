FROM node:18.11.0
WORKDIR /app
COPY package*.json ./
# RUN npm config set registry http://registry.npmjs.org/
# RUN npm config set legacy-peer-deps true 
# RUN npm install --save --legacy-peer-deps
# RUN $ npm config set strict-ssl false
# RUN npm cache clean --force && npm install --force
RUN npm install
COPY . . 
EXPOSE 8080
CMD [ "node", "server.js" ]