FROM node:18

WORKDIR /app

COPY . .

RUN npm ci

RUN npm run build

RUN npm install --global http-server

CMD ["npx", "-y", "http-server", "-p", "8080", "/app/build"]
