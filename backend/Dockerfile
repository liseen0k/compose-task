FROM node:14.16.1
WORKDIR /backend
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3001
ENTRYPOINT npm run start