FROM node:alpine

WORKDIR /app

COPY ./react-app/package.json .

RUN npm install

COPY ./react-app .

CMD ["npm", "run", "start"]