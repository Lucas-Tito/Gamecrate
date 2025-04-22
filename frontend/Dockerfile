# Usar imagem oficial do Node.js
FROM node:23-slim

# Definir diretório de trabalho
WORKDIR /app

# Copiar o package.json e instalar as dependências
COPY package*.json ./
RUN npm install

# Copiar os arquivos restantes do projeto
COPY . .

# Expor a porta onde o Vue.js vai rodar (padrão 8081)
EXPOSE 8081

# Comando para rodar o servidor de desenvolvimento do Vue.js
CMD ["npm", "run", "dev"]
