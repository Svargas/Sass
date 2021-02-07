# Estudos - Sass

## Apanhado de material para uso do estudo do Sassœ

### Instalando ambiente Sass

1. Pra começar tem que está com o node instalado na máquina.

2. Rodar o node na pasta.

```html
npm init -y
```

3. Instala ambiente sass, o save dev não sei pra que serve.

```html
npm install sass —save dev
```

4. cria uma pasta "dist" para distribuição e rodando SASS - CSS

```html
sass --watch src/scss:dist/css
```

5. encontrar no html a pasta src

```jsx
npm install parcel-bundler —save-dev
```

6. deleta a pasta "dist"

7. configura o arquivo "package.json"

Deleta essa parte do "test" no arquivo "package.json"e substitui para comando do "parcel" fazer a mágica

```html
... "scripts": { "test": "echo \"Error: no test specified\" && exit 1" }, ...
```

por

```html
... "scripts": { "dev": "parcel src/index.html", "build": "parcel build
src/index.html" },
```

8. Rodar o "dev" e depois "build" só quando for publicar.

[``html
npm run dev
npm run build

```

👀  obs: criar o arquivo git igonore a pasta node_modules na pasta "src", na hora de publicar rodar o "npm run build" e upar a pasta "dist" - distribuição.
```
