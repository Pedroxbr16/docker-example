# Use Node.js como imagem base
FROM node:18

# Define o diretório de trabalho
WORKDIR /app

# Copia os arquivos necessários
COPY package.json package-lock.json ./

# Instala as dependências
RUN npm install

# Copia o restante do código
COPY . .

# Expõe a porta usada pelo backend
EXPOSE 5000

# Comando para iniciar o servidor
CMD ["npm", "start"]
