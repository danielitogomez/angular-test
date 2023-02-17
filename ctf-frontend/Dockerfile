FROM node:16.16.0
WORKDIR /app
RUN npm install -g @angular/cli@11.2.13
COPY package*.json ./
RUN npm install
COPY . .
RUN ng build --prod
EXPOSE 4200
CMD ["ng", "serve", "--host", "0.0.0.0", "--port", "4200"]
