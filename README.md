# Iniciando e configurando um projeto Node + TypeScript

## 1 Instalar as dependecias para o typescript:
```
npm init -y
npm install -D typescript
npm install -D @types/node
npm install -D ts-node-dev
npm install -D typescript @types/node ts-node-dev
```
================================================================================

## 2 Criar o arquivo tsconfig.json na raiz do projeto:
```
{
  "compilerOptions": {
    "module": "commonjs",
    "target": "es6",
    "rootDir": "./",
    "outDir": "./dist",
    "esModuleInterop": true,
    "strict": true
  }
}
```
================================================================================

## 3 Instalar as dependecias para o express:
```
npm install express
npm install -D @types/express
npm install http-status-codes

```
================================================================================

## 4 Alterar os scripts do package.json:
```
"scripts": {
    "start": "npm run build && node ./dist/index.js",
    "dev": "tsnd index.ts",
    "build": "tsc"
 },
```
================================================================================
