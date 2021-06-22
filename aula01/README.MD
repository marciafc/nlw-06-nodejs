# Notas

```
// Cria projeto com configurações default
yarn init -y

// Add dependência do typescript como dependência de desenv
yarn add typescript -D

// Add dependência do express
yarn add express 

// Instalar tipagem do express como dependência de desenv
yarn add @types/express -D

// Inicializar (primeira vez)
yarn tsc --init 

// desabilitar checkagem strict no tsconfig.json
"strict": false

// Converte ts para js para que o node entenda
// gera um arquivo .js a partir do .ts
yarn tsc

// Executar arquivo js
node src/server.js


// Dependência que automatiza tarefa de converter ts para js
  yarn add ts-node-dev -D
// Criar script em package.json chamando essa dependência ts-node-dev
   "dev": "ts-node-dev src/server.ts"
// Executar app chamando este script  
  yarn dev 
  OU
  npm run dev 

// Abrir terminal  
Control + J 
```

## Endpoints

  - GET localhost:3000/test
  
  - POST localhost:3000/test-post