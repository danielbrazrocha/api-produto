FROM node:14.16.1-alpine3.13
WORKDIR /app
# Copia o package.json e package-lock.json no diretorio corrente
COPY package*.json ./
# baixar dependencias só se houver atualização no package.json
RUN npm install
COPY . .
EXPOSE 8080
CMD ["node", "app.js"]