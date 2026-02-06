FROM node:lts

WORKDIR /app

COPY package.json package-lock.json* ./
RUN npm install

COPY server.js ./

ENV PORT=3000
ENV DATA_DIR=/app/data
EXPOSE 3000

CMD ["node", "server.js"]