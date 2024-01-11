FROM node:alpine as builder

WORKDIR /app

COPY ./react-app/package.json ./

RUN npm install

COPY ./react-app/ ./

CMD ["npm", "run", "build"]


FROM nginx

COPY --from=builder /app/build /usr/share/nginx/html