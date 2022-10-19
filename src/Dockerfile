# Imagem de origem (IMG base)
# é uma boa pratica colocar tag no dockerfile para garantir a indempotência.
FROM node:16.15.0

# Diretorio de trabalho
WORKDIR /app

# fazendo a copia das deps do projeto para o dir corrente 
COPY package*.json ./

# rodando comandos
RUN npm install

# copiando tudo para a pasta /app
COPY . .

# Roda a aplicação
CMD ["node", "server.js"]