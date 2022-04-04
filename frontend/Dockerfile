FROM node:14.16.1
WORKDIR /frontend
COPY  ./frontend/package*.json ./
RUN npm install
COPY ./frontend .
COPY ./backend/package*.json ../backend/
RUN npm install --prefix ../backend
COPY ./backend/common ../backend/common
EXPOSE 3002
ENTRYPOINT npm run start