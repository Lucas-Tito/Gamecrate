# Estágio de build
FROM node:lts-alpine as build-stage
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build

# Estágio de produção
FROM nginx:stable-alpine as production-stage
COPY --from=build-stage /app/dist/frontend /usr/share/nginx/html
# Configuração para SPA (Single Page Application)
COPY nginx.conf /etc/nginx/conf.d/default.conf
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]