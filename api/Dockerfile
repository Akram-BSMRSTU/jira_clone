FROM node:14 AS Production

ENV NODE_ENV=production

WORKDIR /usr/src/api

COPY package.jason .

COPY package-lock.jason .

RUN npm install

COPY . .

RUN npm run build

CMD ["sh", "-c", "npm run start:production"]