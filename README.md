# Configuration Webpack + React + Sass

## 1- Configuration manuelle
```
$ npm init

$ npm install react react-dom --save
$ npm install webpack webpack-dev-server babel-loader babel-preset-es2015 babel-preset-react babel-preset-stage-2 --save-dev
$ npm i -D babel-core
$ npm i -D style-loader css-loader sass-loader node-sass
```
### Créer les fichiers :
- ./webpack.config.js
- ./src/index.html
- ./src/app/index.js
- ./src/app/Components/App.jsx

### Ajouter les  script start, build, build:prod au fichier package.json

```json
"scripts": {
    "start": "npm run build",
    "build": "webpack -d && cp src/index.html dist/index.html && webpack-dev-server --content-base src/ --inline --hot",
    "build:prod": "webpack -p && cp src/index.html dist/index.html"
  }
```

### Exécution
```
$ npm start
```

- server: http://localhost:8080/

## 2 - Clône

```
$ git clone git@github.com:Nedjim/webpack.git
$ cd webpack
$ rm -rf .git
$ git init
$ git remote -v
$ git remote add origin ...
$ npm install
$ npm start
```
- server: http://localhost:8080/



