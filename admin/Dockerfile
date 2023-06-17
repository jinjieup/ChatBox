FROM node:14
WORKDIR /app
COPY package*.json ./
RUN npm i -g install
COPY . .
RUN npm i
RUN npm run build
EXPOSE 3000
CMD [ "npm", "run", "serve" ]
