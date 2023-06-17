FROM node:latest
WORKDIR /app
# COPY package*.json ./
COPY . .
RUN npm i -g pnpm
RUN pnpm i
RUN pnpm dev
EXPOSE 3000
CMD [ "npm", "run", "serve" ]
