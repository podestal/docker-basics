FROM node:20.0.0-alpine3.16
RUN addgroup app && adduser -S -G app app
USER app
WORKDIR /app
COPY package*.json . 
RUN npm install
COPY . .
ENV API_URL = http://api.com
EXPOSE 5173
CMD ["npm", "run", "dev"]