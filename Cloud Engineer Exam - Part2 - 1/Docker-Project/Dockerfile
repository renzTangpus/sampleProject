FROM node:14.16.0-alpine3.13
WORKDIR /app
COPY . .
RUN npm install
ENV API_URL=http:/api.myapp.com/
EXPOSE 5000
RUN ["chmod", "777", "/usr/local/bin/docker-entrypoint.sh"]
CMD ["npm", "start"]