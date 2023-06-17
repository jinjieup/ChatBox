FROM node:latest
WORKDIR /app
COPY . .
# COPY package*.json ./
RUN npm i -g install pnpm
RUN pnpm bootstrap
RUN pnpm i
RUN pnpm run common:prepare
RUN pnpm dev
EXPOSE 3000
CMD [ "npm", "run", "serve" ]
